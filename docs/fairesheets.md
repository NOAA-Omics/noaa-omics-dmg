FAIReSheets Overview
======

![FAIReSheets icon](assets/fairesheets_icon_final.png)

FAIReSheets is a locally run Python CLI application that generates eDNA metadata templates in Google Sheets following the [FAIR eDNA data standard](https://fair-edna.github.io/index.html). It also generates FAIRe-NOAA templates that are ready for [Ocean DNA Explorer](https://www.oceandnaexplorer.org/) submission and compatible with other tools in the FAIRe ecosystem.

**Why this page exists:** Google OAuth app verification requires a public homepage and a dedicated privacy policy URL for apps that request sensitive Google API scopes.

## What FAIReSheets Does

[![Watch tutorial on YouTube](https://img.shields.io/badge/YouTube-Watch%20the%20tutorial-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/dE2g6FswuA0?si=8UNWfRzU_hjMRMFY)

FAIReSheets generates custom FAIRe metadata templates in Google Sheets. The user provides a spreadsheet ID and the application creates the templates using the latest FAIRe checklist. The optional Google Apps Script in the README provides additional custom features like revision history tracking, TSV export, column and row re-ordering, and data validation warnings.

## OAuth Scope and Access

FAIReSheets requests access to the Google Sheets API ([https://www.googleapis.com/auth/spreadsheets](https://www.googleapis.com/auth/spreadsheets)) strictly to read and write formatting, column headers, and data validation templates to a specific Google Spreadsheet ID provided directly by the user.

`SCOPES = ["https://www.googleapis.com/auth/spreadsheets"]`

FAIReSheets does not request broader Google Drive scopes.

## Source Code

Source code, installation instructions, and technical documentation are available in the [FAIReSheets GitHub repository](https://github.com/aomlomics/fairesheets).
