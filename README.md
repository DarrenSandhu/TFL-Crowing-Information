# Transport for London Real-Time Crowding Information

This website provides real-time crowding information for selected TfL (Transport for London) stations. It allows users to select a station and day of the week to view crowding data in both graphical and tabular formats. The website fetches data from the TfL API, processes it, and displays it using dynamic elements such as bar charts and tables.

## Features

- **Real-Time Crowding Data**: Displays up-to-date crowding levels for popular London tube stations.
- **Graphical Display**: Crowding data is shown as an easy-to-read bar chart.
- **Tabular Display**: Crowding data is also provided in a table format, showing specific time bands and their respective crowding percentages.
- **Peak Time Indicators**: Displays the AM and PM peak crowding times for each station.
- **Station and Day Selection**: Users can choose between various stations and days of the week to get specific data.

## Technologies Used

- **HTML**: Markup for the structure of the page.
- **JavaScript**: Implements the functionality to fetch and process the crowding data.
  - Uses `XMLHttpRequest` to retrieve data from the TfL API.
  - **Chart.js**: For rendering the crowding data as a bar chart.
  - **jQuery**: Facilitates easier manipulation of HTML elements.
- **TfL API**: Provides real-time crowding data for tube stations.

## How It Works

1. **User Input**: Users select a station and a day of the week.
2. **API Call**: The website sends a request to the TfL crowding API with the selected station and day.
3. **Data Processing**: The response is parsed, and the crowding percentages are multiplied by 100 to represent them in percentage form.
4. **Display Data**:
   - A **bar chart** is generated, showing crowding across various time bands.
   - A **table** is populated with the same crowding data.
   - AM and PM peak times are displayed as additional information.

## How to Run

1. Open the `TFL_Crowing_Information.html` file in any modern web browser.
2. Use the dropdown menus to select a station and day.
3. Click the "View crowding info!" button to load the data and display the chart, table, and peak times.

## API Key
The API key used in this project is set in the JavaScript code. If you need to change the key, locate this line in the HTML file:

```javascript
xhttp.setRequestHeader("app_key", "cfaeaccfd2b34fd78b97642182097a05");
