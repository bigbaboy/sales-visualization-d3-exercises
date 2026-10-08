# Sales Visualization Exercises with D3.js

An academic front-end visualization project using HTML, JavaScript and D3.js to explore a Vietnamese sales dataset.

## Scope

Standalone Q1–Q12 chart pages. Saved MHTML captures are also included as historical artifacts.

The chart pages explore revenue by product and group, monthly patterns, average sales by weekday/day/hour, order frequencies and customer purchase/spending distributions. The exact aggregation is implemented in each Q-page.

## Run locally

```bash
git clone https://github.com/bigbaboy/LeMinhDat.git
cd LeMinhDat
python -m http.server 8000 --bind 127.0.0.1
```

Open `http://127.0.0.1:8000/Q1.html`. Use a local HTTP server rather than opening the HTML with `file://`, because the charts load CSV data through browser requests.

## Data and files

- `Q1.html`–`Q12.html`: chart implementations.
- `data_ggsheet - data.csv`: shared sales data; preserve the filename and Vietnamese headers.
- D3.js performs filtering, grouping and SVG rendering in the browser.

These setup instructions are based on source inspection, not a full browser smoke test.

## Reading the charts

Start with product/group revenue, then inspect time patterns and order frequencies. A chart labeled as a purchase probability describes observed order frequency within this dataset; it is not a trained predictive model. Check denominator definitions in the relevant page before comparing values across views.

## Related versions

- [Standalone pages](https://github.com/bigbaboy/LeMinhDat)
- [Navigation interface](https://github.com/bigbaboy/LeminhDat48291)
- [Django and relational database version](https://github.com/bigbaboy/221124029109-LeMinhDat-48K29.1)
- [Team sales/segment dashboard](https://github.com/bigbaboy/GroupDV118)

These repositories share related coursework questions. They should be understood as implementation variants, not counted as unrelated commercial projects.

## Future improvements

Add a shared data dictionary, reusable chart utilities, tested metric definitions and screenshots from the running pages. No quantified business impact is claimed.
