# CMU AI-SDM + Meta Repository

## Repo Structure

* [Interactive Version](https://github.com/nikita-jaya/AISDM-Meta-Repo/tree/main/Interactive%20Version) - An interactive streamlit version of situation reports for disasters, including:
	* Winter Storm Fern - 02/2026
	* California Wildfires - 05/2026
* [Situation Reports](https://github.com/nikita-jaya/AISDM-Meta-Repo/tree/main/Situation%20Reports) - Brief documents that are designed to help inform emergency managers (EMs) on people movements after each disaster, including:
	* Winter Storm Fern - 02/2026 (FINISHED)
	* California Wildfires - 05/2026
	* Bordeaux Wildfires - 07/2026 
	* Spokane Fires - 08/2026 (FINISHED)
	* Colombia Earthquakes - 08/2026 (FINISHED)
* [SAM Attempt](https://github.com/nikita-jaya/AISDM-Meta-Repo/tree/main/SAM%20Attempt) - Initial attempts at incorporating Meta's SAM model for disaster management


## Folder Structure: Situation Reports

The structure of these reports is based on the [CrisisReady Situation Report for LA Fires](https://www.crisisready.io/resources/situation-reports/). The situation report utilizes Meta’s Data for Good crisis datasets, which are limited-assess datasets that track population changes through Facebook.

Each folder *always* has following files:

* `data_cleaning.R` or equivalent to clean the Meta datasets and append additional information, such as demographics or Bing tile polygons
* `situation-report.qmd` / `situation-report.pdf` which are the code and report, respectively, for the final deliverables

Occasionally, the folder also has a subset of the following files:
* `references.bib` for additional sources used in the prose or graphics (for the latter, this is usually for tracking the location of the disaster)
* `.mp4` or `.gif` files, which are dynamic visualizations of movement (these are used for initial EDA or the interaction version, if relevant)
* `Previous Work/` folder, which has EDA files and/or previous iterations of the report. These are separate from the version-controlled commits on the final copy because the saved iterations of the report were often submitted for feedback.


## Folder Structure:  Interactive Version

We have also developed a digital version of the situation report using Streamlit. This app allows for interactive maps and customizable plots that can be filtered for specific counties and/or time zones. This app utilizes the same datasets as the situation report: Meta’s Data for Good crisis datasets, which are limited-assess datasets that track population changes through Facebook.

## Folder Structure:  SAM Attempt

We are in the process of developing a workflow that utilizes [Meta's SAM model](https://ai.meta.com/research/sam3/), possibly in conjunction with Meta’s Data for Good crisis datasets. The most up-to-date information can be found in the [README](https://github.com/jaylouissaint/AISDM_Meta/blob/main/SAM%20Attempt/README.md) for this folder.

## Data

Since Meta's datasets are limited-access, the datasets are hosted in Google Drive and are not publicly available.