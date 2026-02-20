# DFW Pilot – Installation Tracking Dashboard

A single-page HTML dashboard for tracking technology installations across vehicle fleets and multiple SCACs. Upload your end-of-shift Excel file every day to see live KPIs, trend charts, and a searchable vehicle table.

## How to Use

1. **Open `index.html`** in any modern web browser (Chrome, Edge, Firefox).
   No server or install required – it runs entirely in the browser.

2. **Upload your daily Excel file**
   - Click *"Choose File"* or drag-and-drop your `.xlsx` / `.xls` / `.csv` onto the upload zone.
   - The first sheet is read automatically.
   - The header row of the file must contain the column names listed below.

3. **Filter & explore**
   - Use the SCAC, Program, Campaign Status, Domicile, and date-range dropdowns to slice the data.
   - Use the search box to find a specific Equipment ID or VIN.
   - Click **Reset** to clear all filters.

4. **Export**
   - Click **Export Filtered CSV** to download the currently visible rows as a CSV file for sharing.

## Required Excel Columns

| Column | Notes |
|--------|-------|
| Equipment ID | Unique vehicle identifier |
| Products Needed | |
| Program | |
| SCAC | Carrier code – used for per-SCAC chart |
| License Plate | |
| VIN | |
| Campaign Status Option (Done/Removed/Replaced) | Drives KPI cards and status chart |
| Domicile | |
| Location Lat/Lon (Per GRIT) | |
| Manufacture | |
| Model | |
| Model Year | |
| Body Type | |
| Fuel Type | |
| Lifecyle state reason | |
| Asset Availability | |
| Communication of Schedule Sent | |
| Scheduled Date | Used for daily trend chart |
| Availability to Start | |
| Availability End Time | |
| Pre-Installation D810 Visit | |
| First Article Required | |
| SOP Need | |
| Cable - Harness Part Number | |
| CANalyzer Needed | |
| VBUS Serial Number | |
| VBUS Install | |
| VBUS/VDR Part Number | |
| DDT Install | |
| DDT Serial Number | |
| DDT/DMS Part Number | |
| DDT/DMS New Bracket Part Number | |
| Haptic Seat - 15 units only | |
| Haptic Seat Part Number | |
| Camera Model Install | |
| New Camera Serial Number | |
| Removed/Returned Camera Serial Number | |
| D450 - 200 Hour Part Number | |
| DR-20 Part Number | |
| External Cameras (D810 Only) | |
| L2 - External Camera Part Number | |
| L2 - External Camera Serial Number | |
| R1  - External Camera Part Number | |
| R1 - External Camera Serial Number | |
| R2  - External Camera Part Number | |
| R2 - External Camera Serial Number | |
| BO  - External Camera Part Number | |
| BO  - External Camera Serial Number | |
| External Camera Bracket Part Number | |
| In-Vehicle Display (D810 only) | |
| Internal Vehicle Display Part Number | |
| Driver Button Install | |
| Driver Activation Button Part Number | |
| Verified In IDMS | |
| CAN Check Status | |
| Acceptable BUS Load Number (goguend) | |
| Pre VBUS Installation Bus Load | |
| Traced BUS Load Number | |
| OTR or In-yard Test Results, if applicable | |
| IDMS Portal Verification | |
| Netradyne SOP Materials Collected | |
| Xirgo Test | |
| Geotab | |
| Truck Wings | |
| MirrorEye | |
| Tractor DriverAssist (TDA) | |

## Dashboard Panels

| Panel | Description |
|-------|-------------|
| **KPI Cards** | Total vehicles · Done · Removed · Replaced · Scheduled · Completion % |
| **Campaign Status** | Doughnut chart of Done / Removed / Replaced / other |
| **Installs by SCAC** | Bar chart – top 20 SCACs by vehicle count |
| **Installs by Program** | Bar chart – top 20 programs |
| **Daily Trend** | Line chart of "Done" installs per scheduled date |
| **Installs by Body Type** | Horizontal bar chart |
| **Vehicle Records Table** | Searchable, filterable table (first 1,000 rows) |

## Dependencies (loaded from CDN – no install needed)

- [Bootstrap 5.3](https://getbootstrap.com/)
- [Bootstrap Icons 1.11](https://icons.getbootstrap.com/)
- [Chart.js 4.4](https://www.chartjs.org/)
- [SheetJS (xlsx) 0.18](https://sheetjs.com/)
