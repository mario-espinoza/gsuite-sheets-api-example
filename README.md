# G Suite Sheets API example

Original Colelab [here](https://codelabs.developers.google.com/codelabs/sheets-api)

Updated example to:

- GoogleApis 52.x.x
- Google Auth library 6.x.x

OAUTH script consent to internal to use the app inside your company

## Possible improvements

Here are some additional ideas for making an even more compelling integration:

### Automatic sync

Rather than have the user click a button to sync, update the spreadsheets automatically whenever orders are changed. You'd need to request [offline access](https://developers.google.com/identity/protocols/OAuth2WebServer#offline) from your users, and keep track of which user owns a given spreadsheet.

### Two-way sync

Allow users to modify order details in the spreadsheet and push those changes back into the application. You could use [Google Drive push notifications](https://developers.google.com/drive/v3/web/push) to detect when the spreadsheet has been updated and the Sheets API's [spreadsheets.values.get](https://developers.google.com/sheets/reference/rest/v4/spreadsheets.values/get) to pull in the updated data.

## Learn More

Read the Google Sheets API developer documentation.
Post questions and find answers on Stackoverflow under the google-sheets-api tag.
