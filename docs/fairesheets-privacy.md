FAIReSheets Privacy Policy
======

![FAIReSheets icon](assets/fairesheets_icon_final.png)

This is the dedicated privacy policy webpage for FAIReSheets.

**Why this page exists:** Google OAuth app verification requires a dedicated privacy policy URL that is separate from the app homepage.

## Google User Data Access

FAIReSheets uses Google OAuth with the Google Sheets API and requests only this scope:

`SCOPES = ["https://www.googleapis.com/auth/spreadsheets"]`

According to the [Google Sheets API scope documentation](https://developers.google.com/sheets/api/scopes), this scope allows the app to view, create, edit, and delete Google Sheets spreadsheets.

In practice, FAIReSheets uses this access only to generate and format metadata templates in the spreadsheet selected by the user.

FAIReSheets does not request broader Google Drive scopes.

## How Google User Data Is Used

FAIReSheets uses Google Sheets data only to provide user-facing template generation and sheet formatting features in the local desktop app.

FAIReSheets does not use Google user data for advertising, resale, profiling, or any unrelated processing.

## Storage and Retention

OAuth credentials are stored locally on the user's machine (for example, `token.json`) and are used by that local app instance to communicate directly with Google APIs.

FAIReSheets does not store Google user data or OAuth tokens on external or backend servers.

## Data Sharing

FAIReSheets does not share Google user data or OAuth credentials with third parties.

## Google API Services User Data Policy

FAIReSheets's use and transfer of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.
