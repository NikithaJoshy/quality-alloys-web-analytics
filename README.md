# Quality Alloys: Website Analytics & Sales Impact

Did a B2B alloy distributor's new website actually drive sales? This project analyzes 15 months of web traffic, engagement, financial, and demographic data to answer that question and recommend changes.

*Texas A&M University, DAEN 400 (Data Analytics & Engineering), Case Study 1, Fall 2025. Individual project.*

## Problem
Quality Alloys, Inc. is a U.S. distributor of industrial alloys sold in small, project-based quantities. The company launched a web presence and ran a promotion to generate leads, but customers could not order online, only request quotes. The goal was to assess whether the website was driving traffic, engagement, and revenue.

## Data
Company-provided workbook (May 2008 to Aug 2009) with weekly and daily site visits, financials, pounds sold, and visitor demographics, split into four periods: Initial, Pre-Promotion, Promotion, and Post-Promotion. *The dataset was provided for coursework and is not included in this repo.*

## Approach
- Time series of weekly visits vs. unique visits with period shading
- Bounce rate and share of new visits by period
- Engagement metrics (page views, pages per visit, average time on site) as a bubble chart
- Regression of weekly profit vs. pounds sold with a confidence band
- Treemap of visits by geographic region

## Key Results
| Period | Page Views | Pages / Visit | Avg. Time on Site |
|---|---|---|---|
| Initial | 32,867 | 2.28 | 80.3 s |
| Pre-Promotion | 31,680 | 2.67 | 95.9 s |
| Promotion | 52,731 | 1.79 | 48.8 s |
| Post-Promotion | 26,155 | 2.18 | 70.0 s |

- The promotion raised page views by about 66% over pre-promotion, but time on site was roughly halved and bounce rate spiked. Traffic did not convert.
- Pounds sold peaked before the promotion (350,000+ lbs) and fell afterward.
- Profit has a clear positive relationship with pounds sold.
- The largest share of visits came from South America (22,616), ahead of North America (17,509). The top referrer was Google Ads (googleads.g.doubleclick.net).

## Recommendations
Improve landing-page engagement and information access, add an online shopping cart, add Spanish-language content for South American visitors, and replicate the Google Ads referral strategy on other platforms.

## Tech Stack
Python, pandas, matplotlib, seaborn, squarify, openpyxl, Jupyter

## Repository Contents
- `notebooks/quality_alloys_analysis.ipynb`: full analysis with charts
- `reports/Quality_Alloys_Report.pdf`: technical report (executive summary, methods, results, limitations, recommendations)
- `reports/Quality_Alloys_Presentation.pdf`: slide deck
