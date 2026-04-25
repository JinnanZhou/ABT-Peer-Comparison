# ABT Peer Comparison

## Project Overview

This project analyses Abbott Laboratories (ABT) in relation to a peer group using financial data from WRDS/Compustat and Python. The aim is to place ABT within an industry context rather than evaluating the company on its own. By comparing sales, net income, profitability, and firm size across similar companies, the project provides a clear example of financial peer benchmarking.

The project combines data extraction, cleaning, summary analysis, and visualisation in a reproducible Python workflow.

---

## Analytical Objective

The main objective of this project is to compare Abbott Laboratories with peer firms and identify patterns in financial performance over time. The analysis focuses on the following questions:

- How does ABT compare with similar firms in terms of scale and financial performance?
- How have average sales, net income, and profitability changed over time within the peer group?
- Does larger firm size appear to be associated with stronger profitability?

This analysis is intended for a business-oriented audience, such as students, financial analysts, or managers interested in industry benchmarking.

---

## Dataset

The dataset was obtained from **WRDS**, using **Compustat annual fundamentals**. WRDS was selected because it is a reliable academic and professional platform that provides standardised company financial data suitable for comparison across firms and years.

### Data characteristics
- Firm-level accounting data from Compustat
- Industry identification using SIC classification
- Annual observations across multiple fiscal years
- Variables suitable for peer comparison and visualisation

### Key variables used
- `sale` — sales/revenue
- `ni` — net income
- `at` — total assets
- profitability measure based on earnings relative to assets
- company identifiers such as ticker, company name, and SIC code where relevant

A broader industry set was first explored, and a narrower peer comparison group was then used to improve relevance.

---

## Tools and Python Libraries

The project was completed in Python using the following tools and libraries:

- `wrds` — to connect to WRDS and extract data
- `pandas` — for data cleaning, filtering, summarisation, and table creation
- `matplotlib` — for charts and visual outputs

---

## Workflow

The analysis followed these main steps:

1. Connect to WRDS using Python.
2. Identify Abbott Laboratories (ABT) and retrieve relevant company information.
3. Build a peer group using industry-related filtering, including SIC-based grouping.
4. Extract annual financial data for the selected firms.
5. Clean and organise the dataset using `pandas`.
6. Calculate average sales, net income, and profitability by fiscal year.
7. Visualise the results using line charts and a scatter plot.

---

## Outputs

The project generated the following main outputs:

### 1. Average Sales by Fiscal Year
A line chart showing how average peer-group sales changed over time.

### 2. Average Net Income by Fiscal Year
A line chart showing yearly changes in average net income.

### 3. Average Profitability by Fiscal Year
A trend chart showing how profitability varied across the sample period.

### 4. Size vs Profitability Scatter Plot
A cross-sectional chart comparing firm size and profitability, showing variation across firms in the peer group.

These outputs were used to summarise both time-series trends and cross-sectional differences.

---

## Main Findings

The analysis produced several clear findings:

- Average sales generally increased over time, suggesting overall growth in scale across the peer group.
- Average net income was more volatile than sales, indicating that revenue growth did not always lead to stable earnings.
- Profitability fluctuated substantially and appeared relatively weak in some years, showing that firm growth and firm efficiency do not always move together.
- Larger firms were not automatically more profitable, as shown in the size-versus-profitability scatter plot.

Overall, the project shows that peer comparison is more informative than viewing a single company alone. It also demonstrates that scale, earnings, and profitability can tell different stories about financial performance.

---

## How to Run

1. Open the Jupyter Notebook file.
2. Run the cells in order.
3. Log in to WRDS when prompted.
4. Execute the SQL queries and analysis cells.
5. Review the generated tables and charts.

**Important note:** This project requires valid WRDS access credentials. Without WRDS access, the data extraction steps will not run successfully.

---

## Files

- `ABT_Peer_Comparison.ipynb` — main notebook containing the code, outputs, and discussion
- `README.md` — project overview and instructions
- `figures/` — optional folder for saved charts if exported

If your notebook filename is different, replace it with the actual file name.

---

## Limitations

This project has several limitations:

- Industry classification is useful for peer selection, but firms with the same or similar SIC code may still differ in business model, strategy, or product mix.
- Accounting-based measures such as net income and profitability can be influenced by exceptional items, acquisitions, restructuring, or accounting choices.
- Average values may be affected by outliers, especially when firms vary substantially in size.
- The analysis is designed as a peer comparison exercise and does not provide a full company valuation or investment recommendation.

These limitations mean the results should be interpreted as an exploratory benchmarking exercise rather than a complete financial assessment.

---

## Possible Improvements

Future improvements could include:

- adding more financial ratios such as ROA or ROE;
- comparing medians as well as averages;
- refining peer selection further;
- highlighting ABT more directly in each visual;
- exporting cleaner charts or building an interactive dashboard.

---

## Author Contribution

I completed the data extraction, cleaning, analysis, and visualisation in Python. I also selected the comparison logic, interpreted the outputs, and structured the project as a business-focused peer benchmarking exercise.

---

## AI Disclosure

I used ChatGPT (OpenAI, accessed on 25 April 2026) to assist with wording, structure, and limited Python clarification. All code execution, analysis, interpretation, and final submitted content were reviewed and completed by me.
