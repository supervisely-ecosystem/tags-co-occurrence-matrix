<div align="center" markdown>
<img src="https://i.imgur.com/5p80yOt.png"/>

# Tags Co-Occurrence Matrix

<p align="center">
  <a href="#Overview">Overview</a> •
  <a href="#How-To-Use">How To Use</a>
</p>


[![](https://img.shields.io/badge/supervisely-ecosystem-brightgreen)](../../../../supervisely-ecosystem/tags-co-occurrence-matrix)
[![](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://supervisely.com/slack)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/supervisely-ecosystem/tags-co-occurrence-matrix)
[![views](https://app.supervisely.com/img/badges/views/supervisely-ecosystem/tags-co-occurrence-matrix.png)](https://supervisely.com)
[![runs](https://app.supervisely.com/img/badges/runs/supervisely-ecosystem/tags-co-occurrence-matrix.png)](https://supervisely.com)

</div>

## Overview

App takes images project (or dataset) as an input and produces an “Interactive co-occurrence matrix” that has the following dimensions: `row_number = number of tags`, `col_number = number of tags`. Each cell of the matrix shows how often a pair of tags (say person and car) appears together (how many images that simultaneously contain at least 1 person and at least 1 car). Each cell is clickable to open corresponding images.

Additional comments:
- This app is good for data exploration since it allows to see a big picture (co-occurrence statistics) as well as to navigate to the images of interest
- This App might be used to find “suspicious annotations”. If annotator has confused the tag, we might see it as an “unexpected value” in the cell of “coexistence matrix”
- Gradient based colors of the matrix’ cells might be useful (will be added in next version)

<img src="https://i.imgur.com/Zm8va1F.png"/>

## How To Use

**Step 1:** Add app to your team from Ecosystem if it is not there

**Step 2:** Run app from the context menu of images project or dataset: `context menu` -> `Reports` -> `Tags Co-Occurrence Matrix`

<img src="https://i.imgur.com/xcMc6pe.png" width="500px"/>

**Step 3:** Wait until the app is started, press `Open` button in `Workspace tasks`. You don't need to wait untill all images are processed: if open button is enabled then click it.

<img src="https://i.imgur.com/E3AnaLN.png"/>


**Step 4:** Explore you data with interactive table: click on cells to access corresponding images and open them in labeling UI.

**Step 5:** App saves link to report to team files: `/reports/tags-co-occurrence/<project id>_<project_name>.lnk`. Link to generated report also available in task output column. 

**Step 6:** Stop application once you finished with it. App can be stopped from tasks list or from application UI.

Example of the results:
Stop from App UI  |  Stop from workspace tasks page
:-------------------------:|:-----------------------------------:
![](https://i.imgur.com/6ZovGTo.png)  |  ![](https://i.imgur.com/PLFUHmB.png)
