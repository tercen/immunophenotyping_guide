# Adjusting Events and Channels

In this lesson we will open analysis blocks and adjust relevant settings to control which channels and events are included in the analysis.

We will set up browser tabs to review how they impact the visualisations.

## Clone the workflow

![Screenshot](docs/images/2_clone_workflow.jpg)

In order to compare our changes to the original we will clone the workflow.

Press the Clone Button

Click **Next** to select the team.

Click **Next** to select the project

*Note: If you have followed this tutorial you should not have to change the automatic suggestions. Be aware that if you created this tutorial into a Team then you may have to change selections here.*

Rename the workflow to "Analysis Settings Changed".

Press OK

Right click the Immunophenotyping Guide link in the breadcrumb.

Select "Open in a new Tab"

Click the **Flow Immunophenotyping - Phenograph** link to open it.

Now you can change tabs on your browser to compare changes.

## Adjust Channels in the analysis

Select the **Analysis Settings Changed** workflow on your browser tab.

Double Click the **Data pre-processing** box.

The view panel will open.

Choose **Channel Selection and Downsampling**

A data step will open.

### Remove a Channel

Press the Reset button to allow us to modify settings.

Click the chevron on the filters section and select Exclude QC channels.

This filter is a list of all channels currently excluded from the analysis.

To Remove a channel from the analysis we add it to the exclusion list.

Press the plus button.

A new line will be created.

Change the *NaN* value to **CD38**

### Add a Channel

To add an excluded channel into our analysis remove it from this list.

For the **FSC-A** line.

Press the minus button.

Press OK.

Press Save.

Return to **Analysis Settings Changed** workflow using the Breadcrumb.

## Downsampling

Downsampling is the process of reducing the amount of data for analysis. This is done by systematically selecting a subset of the data at a lower rate than the original.

Downsampling can give you a quick analysis result by processing less data. Useful for forming an opinion on how the data looks before submitting the full amount for a long running calculation.

Downsampling can also balance an analysis across samples which do not have the same number of data points.

From the Analysis Settings Changed workflow

Double Click the **Data pre-processing** box.

The view panel will open.

Choose **Channel Selection and Downsampling**

The data step will open again.

Press the Reset button to allow us to modify settings.

Downsampling is controlled by two types of filter.

Choose the filter that best represents your needs.

### Downsampling # Events

This is a whole number setting for the maximum events to be included from each file.

Files with less events than this setting will have all events included and files with more will be restricted.

To modify.

Click the chevron on the filters section and select **Downsampling # Events**.

Change the value to **1000**

### Downsampling Percentage

This is a proportionate setting for the maximum events to be included from each file.

This setting takes a balanced approach based on the file with smallest number of events.

For example.

If there are two FCS files. One with 1000 events and one with 10000 events and the downsampling is set to 80%.

Both files will be reduced to 800 events for calculation. The smaller file dictates the number calculated.

To modify.

Click the chevron on the filters section and select **Downsampling Percentage**.

Change the value to **40**

## Re-Run the Workflow

Press OK.

Press Save.

Return to **Analysis Settings Changed** workflow using the Breadcrumb

Press **Run All**

## Compare changes

Using the tabs on your browser open the report window in both workflows.

Compare **Channel names and descriptions** and **Event Count (filtered data)**.
