# CRM Donor Analytics & Power BI Dashboard

## Summary

In this project I analyzed a CRM donor dataset, cleaned and feature-engineered the data using Python, and built a Power BI dashboard to surface revenue, donor-segmentation, engagement, and geographic insights. The final output is a cleaned CSV that I use as the data source for the dashboard.

## What I did

- Cleaned raw donor data (date parsing, duplicates, basic validation)
- Converted `LastDonationDate` to datetime and extracted `Year` and `Month`
- Created a `Segment` column based on `TotalAmountDonated` (High, Medium, Low)
- Calculated KPIs and exploratory metrics (total revenue, top donors, revenue by segment)
- Exported the processed dataset for Power BI and built interactive visuals

## Tools

- Python (pandas, numpy)
- Power BI (report and visuals)
- Git for version control

## Power BI Dashboard (what I built)

- KPI cards: Revenue, Customers, Donations, Engagement
- Revenue trend over time (monthly) using `Year` and `Month`
- Revenue by customer segment (`Segment`)
- Customer activity (Total Gifts) by segment
- Revenue by state (choropleth / bar chart)
- Top donors table (top 10 by `TotalAmountDonated`)
- Filters / slicers: `Segment` and `Year` for interactive exploration

## Key steps and why I did them

- Data cleaning: I standardized dates and removed obvious duplicates so visuals and aggregates are reliable.
- Feature engineering: I added `Year` and `Month` to speed up time-based aggregation in Power BI and to avoid heavy DAX transformations.
- Segmentation: I created `High`, `Medium`, and `Low` segments so stakeholders can focus on retention and growth strategies for the segments that matter most.
- Exporting: I saved the processed CSV so the Power BI report can load a stable, reproducible dataset.

## Key insights

- Revenue concentration: High-value donors generate the majority of revenue — retaining this small group is high priority.
- Time trends: Monthly revenue shows clear peaks and troughs that inform campaign timing and seasonal planning.
- Engagement correlation: Donors with higher engagement scores donate more on average, so increasing engagement should raise revenue.
- Geographic patterns: A handful of states account for a disproportionate share of revenue, highlighting regional focus areas.

## How to reproduce

1. Install Python dependencies (if not already available):

```powershell
pip install pandas numpy
```

2. Run the notebook to regenerate the processed CSV:

```powershell
# from the project root
python -m pip install -r requirements.txt  # optional if you maintain requirements
# open and run notebooks/crm_analysis.ipynb in Jupyter or VS Code
```

3. In Power BI Desktop: `Get Data` → `Text/CSV` → select `data/processed/cleaned_crm_data.csv` and build visuals.

## Project structure
```
crm-powerbi-dashboard/
├── data/
│   ├── raw/                  # original dataset
│   └── processed/            # cleaned output (cleaned_crm_data.csv)
├── notebooks/                # analysis notebook
├── dashboard/                # Power BI files and report
├── images/                   # screenshots and preview images
└── README.md
```

## Author
Asres Gamu Yelia — Power BI Specialist | KPI Dashboards & Business Insights

