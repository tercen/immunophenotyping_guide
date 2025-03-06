# How to Run the immunophenotyping template

This tutorial explains how to start a project and run the immunophenotyping template, 

Templates are pre-defined workflows that are saved into Tercen for quick loading.

They provide standardisation of analysis and help make experiments reproducible.

This chapter will use pre-prepared data (FCS files and an annotation file) to demonstrate the concepts.

## Create a project

![Screenshot](docs/images/1_New_Project.jpg)

Click the New **Project** Button.

Name it "Immunophenotyping Guide"

Press OK.

## New workflow

![Screenshot](docs/images/1_Begin_Analysis.jpg)

To begin an analysis click **New Workflow**

Choose - **Flow Immunophenotyping - Phenograph**

![Screenshot](docs/images/1_choose_template.jpg)

Press Ok

## Run an analysis

The workflow canvas will show the immunophenotyping workflow.

It has sections to perform different functions.

- Importing files.
- Quality Control and Normalisation of Data.
- Analysis algorithms for clustering and dimension reduction.
- Reports

![Screenshot](docs/images/1_workflow.jpg)

Press **Run All** to begin analysis

Tercen will ask you to assign files to be analysed.

Sample files have been uploaded in advance to the Tercen Library.

Use the *Main Library* and *flow cytometry* tags to narrow down the selection.

Choose ***OMIP=-69 - FCS Files (10k Events).zip***

![Screenshot](docs/images/1_fcs_files.jpg)

Press OK.

This Template uses an annotation file to describe treatment conditions.

Use the Tags and search bar to find and select ***OMIP-069 - Sample Annotation.txt***

![Screenshot](docs/images/1_annotation.jpg)

Press OK.

The workflow will being analysis and will show a spinning icon on the step is is processing as well as progress bars along the bottom of the screen.

When a step has finished it will display a Green Dot.

When the workflow has completed all analysis **Save** the workflow.

## Report Tab

Data Pre-processing:
Read FCS - An overview of the main data in the files which were uploaded.
Channel Names and descriptions
Event Count
Marker Distribution (logicle)
Marker Distribution (z value)


---

## Examine the data

![Screenshot](docs/images/1_local_toolbar.jpg)

Click a step to bring up the local toolbar.

Select **Edit**.
