# Medicine Use in Australia — FIT3179 Assignment 2

## Status
**Starter prototype, not final submission.** Four narrative sections and two working Vega-Lite charts from the uploaded ABS NHSDC01 workbook. Other chart positions are explicit placeholders because the AIHW HWE-098/HWE-099 source files were not attached in the current runtime. No PBS figures or geographic boundaries have been invented.

## Run locally
From this folder: `python -m http.server 8000`
Open `http://localhost:8000`. Do not open index.html directly using file://, since Vega-Lite loads CSV and JSON by URL.

## Project layout
- `index.html`: single scrolling dashboard
- `css/styles.css`: responsive editorial layout
- `js/*.vg.json`: readable Vega-Lite specs
- `data/chronic_conditions.csv`: 56? observations extracted from ABS NHSDC01, Table 1.3; missing years excluded

## Before submission
1. Add source AIHW HWE-098 and HWE-099 workbooks and verify definitions/units; transform to small CSVs.
2. Build national, age, geographic and socioeconomic charts.
3. Obtain correct Australian state and LGA geographic boundaries; check LGA code vintage and joins.
4. Verify **at least 10 charts**, **at least 8 distinct advanced idioms**, and **3 different map idioms**. Repeated idioms are not distinct.
5. Use only defensible analytical comparisons; don't equate PBS dispensing with actual medicine consumption or disease prevalence.
6. Add annotations, sources, method notes, final sketch PDF link, and required What/Why/Who/How description.
7. Deploy repository through GitHub Pages; ensure JSON specs are accessible and data files are a few MB total.

## Data provenance
ABS National Health Survey 2022, Table 1.3 — unadjusted proportions (all ages) for selected indicators. Source: https://www.abs.gov.au/statistics/health/health-conditions-and-risks/national-health-survey/latest-release
