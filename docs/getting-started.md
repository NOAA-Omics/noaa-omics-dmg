Getting Started
=====

## Key Requirements for Omics Data 

In accordance with the [NOAA Plan for Increasing Public Access to Research Results (PARR)](https://www.glerl.noaa.gov/review2016/reviewer_docs/NOAA_PARR_Plan_v5.04.pdf) and the new [NAO 212-15B Data Management Handbook](https://sites.google.com/noaa.gov/noaa-data/handbook), NOAA-funded digitally formatted scientific data must be made publicly visible and accessible in a timely manner, in a machine-readable format using non-proprietary standards, and with the metadata necessary to find and properly use the data.  

To meet these requirements, every NOAA Omics project should have a Data Management Plan. The Data Management requirements are listed below:  

1. Fill out a **[Data Management Plan template](https://noaa-omics-dmg.readthedocs.io/en/latest/study-data-templates.html)** to describe your [data management workflow](https://noaa-omics-dmg.readthedocs.io/en/latest/getting-started.html#data-management-workflow). 
2. **Omics Data Guidelines:** Submission of [omics data](https://noaa-omics-dmg.readthedocs.io/en/latest/omics-data-guidelines.html) to the appropriate public data repository (e.g., raw sequence data to NCBI).
3. **Metadata Guidelines:** Projects including [environmental measurements](https://noaa-omics-dmg.readthedocs.io/en/latest/metadata-guidelines.html#submitting-metadata-and-environmental-data-to-repositories) (e.g., cruises, mesocosm experiments) must submit metadata and environmental data to [NCEI](https://www.ncei.noaa.gov/). For all projects, relevant metadata and data products not submitted in (#2) should be submitted to the appropriate public archived repository. Some examples of metadata include contextual info about the project, protocols, and bioinformatics code. 
4. Persistent digital object identifiers (DOI) or accession numbers generated in (#2) and (#3) must be **[cross-linked](https://noaa-omics-dmg.readthedocs.io/en/latest/omics-data-guidelines.html#archiving-and-cross-linking)** so that all data and metadata from a project can be discoverable.  

![DMG fig](assets/20240204_mermaid_eDNA_workflow_ndmc.png)

![DMG fig](assets/noaa_data_lifecycle.png)

## Data Management Workflow

A successful data management workflow will contain the following steps:

* **Start early** – Develop your [data management plan](https://noaa-omics-dmg.readthedocs.io/en/latest/dmp-template.html) (with help from this guide) at the proposal stage.
* **Identify your data type(s)** – The types of omics data you generate (e.g., amplicon, metagenomic, proteomic) dictate [which standards are available](https://noaa-omics-dmg.readthedocs.io/en/latest/omics-data-guidelines.html) and some of the metadata you'll want to collect (e.g., the sample preparation data).
* **Identify your environment(s)** – If your samples came from the environment (e.g., seawater) or an environmental system (mesocosm), there are specific parameters you'll want to collect (e.g., temperature, salinity). If your samples are from an experimental system, you'll want to capture your experimental factors and possibly also ambient conditions.
* **Locate checklists and templates** – Find the relevant [standards, checklists and templates](https://noaa-omics-dmg.readthedocs.io/en/latest/study-data-templates.html) for your data type(s) and environment(s). 
* **Complete your metadata** – As soon as you have sample or experimental metadata, start recording it in the appropriate format. Make sure to backup original and formatted metadata files. NOAA's project metadata format requirement is ISO 19115-2.
* **Identify (meta)data repositories** – List the relevant and required data and metadata repositories, then verify submission instructions and user accounts.
* **Share and archive your code** -  If your project includes code, make it publically available on services like Github, [include a license](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository), and archive it using a data archive tool like [Zenodo](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content).
* **Submit your data!** – Recommended timeline for submission is one year after the project end date (NOAA intramural PIs), two years after the project end (extramural PIs), or before a paper is published using these data (whichever is sooner).



