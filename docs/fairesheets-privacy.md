FAIReSheets Privacy Policy
======

![FAIReSheets icon](assets/fairesheets_icon_final.png)

This is the dedicated privacy policy webpage for FAIReSheets.

**Why this page exists:** Google OAuth app verification requires a dedicated privacy policy URL that is separate from the app homepage.

## Google User Data Access

FAIReSheets requests access to the Google Sheets API ([https://www.googleapis.com/auth/spreadsheets](https://www.googleapis.com/auth/spreadsheets)) strictly to read and write formatting, column headers, and data validation templates to a specific Google Spreadsheet ID provided directly by the user.

`SCOPES = ["https://www.googleapis.com/auth/spreadsheets"]`

FAIReSheets does not request broader Google Drive scopes.

## How Google User Data Is Used

FAIReSheets uses Google Sheets data only to provide user-facing template generation and sheet formatting features in the local Python CLI application.

FAIReSheets does not use Google user data for advertising, resale, profiling, or any unrelated processing.

## Data Protection Mechanisms

All data processing occurs locally on the user's machine. FAIReSheets does not host, transmit, or process Google user data on any external third-party servers. All communication with Google APIs is secured via standard HTTPS encryption.

## Data Retention and Deletion

### Spreadsheet Data

FAIReSheets does not retain, store, or log any Google Spreadsheet user data. Data is held in volatile memory only for the duration of the execution of the script and is permanently discarded as soon as the application process ends.

### Auth Data

To prevent users from needing to re-authenticate on every launch, standard OAuth credentials (e.g., `token.json`) are stored strictly locally on the user's machine. These tokens are never transmitted to or stored on any external servers.

OAuth client credentials (e.g., `client_secrets.json`) used to identify the FAIReSheets application to Google are also stored locally on the user's machine and do not contain or transmit any Google user data.

## Data Sharing

FAIReSheets does not share Google user data or OAuth credentials with third parties.

## Limited Use Disclosure

The use of raw or derived user data received from Workspace APIs will adhere to the [Google User Data Policy](https://developers.google.com/workspace/workspace-api-user-data-developer-policy), including the Limited Use requirements.

FAIReSheets's use and transfer of information received from Google APIs also adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy).
