Omics Data Guidelines
======

Omics datasets should be sent to the relevant long-term data repository in accordance with the publication requirements of the field of study. While NCEI can be used to curate some small omics datasets (< ~20 GB), it is not easily searchable nor does it allow for critically important interactive querying (e.g., BLAST), and so should not be the lone repository for omics data if other options apply. Raw data (e.g., FASTQ files from the sequencing center) should be submitted to a repository for proper archiving. Data analysis products (e.g., MAG/genome assemblies) are useful to the scientific community, and should be submitted to relevant repositories. We offer guidelines for archival locations for omics datasets below and in [Table 2](https://github.com/aomlomics/omics-data-management/wiki/3-Study-Data-Templates#submitting-processed-omics-data).

## Repositories

Recommended destinations for different data types

### Table 1 - Data repositories

Suggested formats and destinations repositories for common environmental omics datasets. 

Data type | Data formats (non-exhaustive) | Repository
-- | -- | --
DNA reference sequences | GenBank format | [NCBI GenBank](https://www.ncbi.nlm.nih.gov/genbank/submit/)
DNA sequence data (amplicon, metagenomic, RAD-Seq) | Raw FASTQ | [NCBI SRA](https://www.ncbi.nlm.nih.gov/sra/docs/submit/)
Amplicon Sequence Variants | Reference FASTA | [NCEI](https://www.ncei.noaa.gov/archive)
RNA sequence data (RNA-Seq) | Raw FASTQ | [NCBI SRA](https://www.ncbi.nlm.nih.gov/sra/docs/submit/)
Functional genomics data (quantitative gene expression, ChIP-Seq, HiC-seq, methylation seq) | Metadata, processed data (e.g., raw read counts) raw FASTQ | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/info/submission.html) (raw data submitted to NCBI SRA for you)
RNA transcript assemblies | FASTA or SQN file | [NCBI TSA](https://www.ncbi.nlm.nih.gov/genbank/tsa/)
Genome assemblies | FASTA or SQN file, optional AGP file to orient scaffolds | [NCBI WGS](https://www.ncbi.nlm.nih.gov/genbank/genomesubmit/)
Quantitative PCR data | Tab-delimited text | [NCEI](https://www.ncei.noaa.gov/archive)
Mass spectrometry data (metabolomics, proteomics) | Raw mass spectra, MZML, MZID | [ProteomeXChange](https://www.proteomexchange.org/), [Metabolomics Workbench](https://www.metabolomicsworkbench.org/)
Feature observation tables and feature metadata | BIOM (HDF5) format (feature observation tables), tab-delimited text (feature metadata) | [NCEI](https://www.ncei.noaa.gov/archive) (size permitting), [Zenodo](https://zenodo.org/), or [Figshare](https://figshare.com/)
Reference database | FASTA (sequences) and TSV (taxonomy) | Custom public server with DOIs, or repositories such as [Zenodo](https://zenodo.org/), [FigShare](https://figshare.com/), or [Dryad](https://datadryad.org/stash)

Notes on data formats:

* Tab-delimited text files should contain a single row at the top containing column headers. Column headers should be written in camelCase or with_underscores (no spaces) with units included in the column headers.
* Tab-delimited text files can be created as Microsoft Excel or Google Sheet files, edited, and then saved as tab-delimited text (.txt, Excel) or tab-separated values (.tsv, Sheets), which are the same except for the extension.

## Storage & Backup

Best practices for storage and backup of 'omics data should ensure that the data files are associated with their metadata and backed up securely.

### Raw data

Upon receipt of raw sequencing data, FASTQ files should be immediately stored in two locations (e.g., a local drive for analyses and on the NOAA Google Drive). The location of these files and their [metadata](https://github.com/aomlomics/omics-data-management/wiki/4-Metadata-Guidelines) (e.g., file name, associated project, sequence submission date) should be recorded on a Google Spreadsheet. This spreadsheet should be backed up on a regular basis by downloading it as a tab-delimited file and saving to an external drive. 

Storage locations of raw sequence data should have a regularly scheduled backup plan (e.g., RAID on server drives, external backup of Google Drive).

### Intermediate and processed data files

Depending on your 'omics method, you will generate various types of intermediate and final processed files. For files produced by analyses that are computationally or time-intensive (e.g., trimmed FASTQ files, ASVs, assembled RADseq loci), it is a good idea to backup them up in a second location until the project is completed or the files are uploaded to a repository such as Dryad, Zenodo, or Figshare.

## Archiving and cross-linking

All NOAA ‘omics projects that are eligible for NCEI should include a project submission to the [National Centers for Environmental Information (NCEI)](https://www.ncei.noaa.gov/), and provide a README file locating where all products of that project have been submitted. This file should contain a description of the data and a link to a persistent digital object identifier (DOI) or NCBI accession number. This file should include include links to all raw data, metadata, data analysis products, and code used for the ‘omics project, including a self-referential link to the NCEI project submission where the README file is found. 

This NCEI accession number can be cross-listed in other repositories containing the project's data. For example, you can provide a link to the NCEI project in the "Related Resources" section of an NCBI BioProject.

An additional organized and accessible data archive can further support reproducibility of a project. This archive can be hosted on Figshare, Dryad, or Github and archived with Zenodo. It should include cross-listed repository links or files for all raw data, metadata, data analysis products, code, and any research products (manuscripts, figures, ect.). Optionally, it can also include details on lab or field protocols.  

The [AOML ’Omics](https://github.com/aomlomics/) GitHub organization contains the repository [Datasets](https://github.com/aomlomics/datasets) that lists the datasets generated by AOML ’Omics and links to the primary data location (BioProject, ProteomeXchange, or NCEI). It can be viewed as a [GitHub Page](https://aomlomics.github.io/datasets/), which is more user-friendly than a repository page. ’Omics users can edit the README.md file (containing the table of datasets) directly from a web browser (command-line Git is not required).
