# Working with Clusters

This chapter explains the settings that control the clusters found by the Phenograph algorithm and how they are represented by the UMAP algorithm.

## Clone the workflow

Take another copy of the original workflow.

Press the Clone Button

Click **Next** to select the team.

Click **Next** to select the project

*Note: If you have followed this tutorial you should not have to change the automatic suggestions. Be aware that if you created this tutorial into a Team then you may have to change selections here.*

Rename the workflow to "Cluster Settings".

Press OK

Right click the Immunophenotyping Guide link in the breadcrumb.

Select "Open in a new Tab"

Click the **Flow Immunophenotyping - Phenograph** link to open it.

Now you can change tabs on your browser to compare changes.

## Adjusting Phenograph

PhenoGraph is a graph-based clustering algorithm that constructs a k-nearest neighbour graph. It is widely used for high-dimensional single-cell data analysis.

Select the **Cluster Settings** workflow on your browser tab.

Double Click the **Clustering and Dimension Reduction** box.

The view panel will open.

Choose **Clustering: Phenograph**

![Screenshot](docs/images/3_Clustering_phenograph.jpg)

A data step will open.

Press **Reset** to allow modification.

Open the **Settings Panel** by clicking the tab.

![Screenshot](docs/images/3_phenograph.jpg)

### k value

This is the stringency parameter it adjust how clusters will appear on any visualisation.

This can help with defining separation from other clusters.

A higher value means larger clusters.

A lover value means smaller clusters.

Set **k** to 15

### Seed

Controls randomness in the calculations made by the algorithm.

By re-running the algorithm with different seed values you can test how reliably it is finding clusters. If different seed values still produce the same graph then the algorithm is stable.

Set **seed** to 29.

## UMAP

UMAP (Uniform Manifold Approximation and Projection) is a nonlinear dimensionality reduction technique that preserves global and local structures, making it useful for visualizing high-dimensional data.

Double Click the **Clustering and Dimension Reduction** box.

The view panel will open.

Choose **Dimension Reduction: UMAP**

A data step will open.

Press **Reset** to allow modification.

Open the **Settings Panel** by clicking the tab.

Two settings influence how clumped together or separated the clusters are in the visualisation.

![Screenshot](docs/images/3_UMAP.jpg)

### Spread

Set spread to 2

## min-dist

Set min-dist to 0.75

*Note: UMAP also uses a seed to control randomness. You can perform the same stability checks for UMAP with this setting.

Press **Save**.

## Configure how plots appear

Tercen allows you to change colour palettes and labels on graphs.

Select the **Cluster Settings** workflow on your browser tab.

Double Click the **Clustering and Dimension Reduction** box.

The view panel will open.

Choose **UMAP vs. Marker Expression**

Prese **Reset** to allow modification.

### Plot Layout Settings

In the settings tab.

![Screenshot](docs/images/3_UMAP_plot.jpg)

Change title to "UMAP Marker - Jet"

Change **xlab** to "UMAP A"

Change **ylab** to "UMAP B"

There are other settings for sizes, fonts and notation.

### Colour Palette

Select the *Palette** tab.

Change the palette to "Jet".

Press **Save**

## Re-Run the Workflow

Return to **Cluster Settings** workflow using the Breadcrumb

Press **Run All**

Press Save.

## Compare changes

Using the tabs on your browser open the report window in both workflows.

Compare how the visualisations have changed from the original.

Graphs to compare.

- UMAP by PhenoGraph Cluster.
- UMAP vs. Marker Expression.
