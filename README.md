# Electric Vehicle Market Performance & Insights

An interactive project based on the user-supplied `ev_market_test.csv`, with a local browser dashboard, packaged Tableau workbook, project report, data dictionary, and reproducible build/presentation guides. The SkillWallet screenshots provide assignment context and a visual reference; example text about other datasets is not used as evidence for this EV analysis.

## Start the interactive dashboard

1. Keep `dashboard.html`, `ev_market_test.csv`, and `Start_Dashboard.bat` in the same folder.
2. Double-click `Start_Dashboard.bat`. It opens the dashboard at `http://127.0.0.1:8765` and serves the CSV locally. Keep the command window open while using the dashboard; close it to stop the server.
3. Filter by model year, market region, vehicle category, battery type, or manufacturer text. Select **Reset filters** to clear the filters.

Requires Python 3 on Windows. If the port is already in use, close the other local server or change `8765` in the batch file and dashboard URL.

## Dashboard contents

Six KPI cards show distinct manufacturer labels, distinct model names, reported annual sales, average source rating, average driving range, and average battery capacity. The views compare sales by model year, manufacturer, and category; record counts by manufacturing country; battery range and capacity; capacity versus range; and ratings by category. The shared filters recalculate metrics and charts.

## Source and interpretation

The CSV contains 100,000 rows and 37 columns, with model years 2018–2026, 200 manufacturer labels, 15 vehicle categories, 7 market-region labels, and 10 manufacturing-country labels. It contains 9,511 blanks across five fields: battery cycle life (2,028), resale value (3,057), infotainment screen size (1,506), reported annual sales (989), and customer rating (1,931). Missing values are excluded from the relevant aggregate.

The filename says `test`, manufacturer labels appear synthetic, country and region representations look unusually balanced, and no provenance is supplied. Treat this as simulated/test data. The reported sales sum (772,608,124 across nonblank rows), mean range (324.3 km), and mean rating (4.08/5) describe this file only. Model Year is not transaction date. Sales rankings are not market share, and rating values are not verified customer sentiment.

## Files

- `Project_Report.md` — complete project summary, dataset notes, dashboard interpretation, run instructions, and handoff status.
- `dashboard.html` — interactive local browser dashboard.
- `EV_Market_Performance_Insights_Complete.twbx` — Tableau packaged workbook with an extract, an overview dashboard, and eight worksheet views: Manufacturer Sales, Sales by Category, Sales by Model Year, Sales by Manufacturing Country, Battery Type Sales Mix, Average Rating by Category, Average Range by Battery, and Average Capacity by Battery.
- `EV_Market_Performance_Insights_Complete.twb` — editable Tableau workbook definition.
- `ev_market_test.csv` — supplied source data copy.
- `Data_Dictionary.csv` — field descriptions, units, types, and missing counts.
- `Project_Plan.md` — assignment personas, eight epics/fourteen tasks, acceptance criteria, and architecture.
- `Scene_Storyboard.md` — seven-scene narrative and timed 5–7 minute walkthrough.
- `Tableau_Build_Guide.md` — calculations, views, filters, caveats, and Tableau steps.
- `Start_Dashboard.bat` — local Windows launcher.

## Tableau and external handoff

Open `EV_Market_Performance_Insights_Complete.twbx` in Tableau Public or Tableau Desktop; its extract is packaged. The Tableau dashboard currently places the three core sales views; the additional five analysis views are available as standalone worksheets. The local browser dashboard presents all analysis themes together. This local package does not claim that Tableau Public, Flask hosting, a demo recording, or SkillWallet links have been published or submitted.
