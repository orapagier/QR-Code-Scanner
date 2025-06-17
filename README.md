# QR Code Scanner with Google Sheets Integration

A web-based QR code scanner that automatically saves scanned data to Google Sheets.

## Features
- Real-time QR code scanning using device camera
- Automatic saving to Google Sheets
- Scan history tracking
- Statistics dashboard
- Mobile-friendly responsive design

## Setup Instructions

### 1. Configure Google Sheets API
1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select existing one
3. Enable the Google Sheets API
4. Create an API key and restrict it to Google Sheets API

### 2. Prepare Your Google Sheet
1. Create a new Google Sheet
2. Make it publicly accessible (Share → Anyone with link can edit)
3. Note the Sheet ID from the URL

### 3. Update Configuration
Edit `index.html` and replace these values in the CONFIG object:
```javascript
const CONFIG = {
  GOOGLE_SHEETS_API_KEY: 'your_actual_api_key_here',
  GOOGLE_SHEET_ID: 'your_actual_sheet_id_here',
  SHEET_NAME: 'Sheet1'
};
