# Estonian Housing Affordability Dashboard

An interactive two-page dashboard showing how many m² of housing one average monthly salary buys in each Estonian county, 2005–2026.

## Key questions
- How have housing prices per m² and salaries changed over time?
- How many m² can one monthly salary buy, and how does this differ by county?
- How are housing prices related to interest rates and inflation?

## Key findings
- Average housing price rose from €321/m² (2005) to €1,116/m² (2026, Q1–Q2), +247.6%; the average salary rose from €432 to €1,795.
- Affordability differs strongly by county: about 0.8 m² per monthly salary in Harju vs 4.1 m² in Jõgeva (2005–2026 average). Estonian average: 1.66 m².
- Estonian affordability fell to 1.45 m² in 2022, after rising interest rates and inflation, and has partly recovered (1.61 m² in 2026).

## Dashboard
- **Page 1:** housing prices, prices vs. salaries, price and salary levels by county, interest rate, CPI
- **Page 2:** salary vs. price scatter, prices vs. interest rates, affordability by county, trend and year-by-year matrix
- Year and county filters with a "RESET" button

## Data sources
- Housing prices: [Maa-amet](https://maaamet.ee/)
- Salaries (PA21, PA004, PA117) and CPI (IA002): [Statistikaamet](https://www.stat.ee/)
- Housing loan interest rates: [Eesti Pank](https://www.eestipank.ee/)

## Method
- Affordability = average salary ÷ average housing price per m².
- Interest rate = quarterly average of monthly values (EUR loans).
- CPI growth = average CPI of the selected period ÷ average CPI of its first year.
- Prices and salaries are nominal (not adjusted for inflation).

## Limitations
- 2026 covers Q1–Q2 only.
- County prices are simple averages; small counties (e.g. Hiiu) have few transactions.

## Files
- `Housing_Affordability_in_Estonia.html`: interactive dashboard (open in a browser)
- `Housing_Affordability_Dashboard_Explained.pdf`
- `Housing_Affordability_Dashboard.pdf` / `.docx`: documentation of the dashboard

## Tools
Power BI, DAX, SQL (DBeaver), Python. The web version was made with the help of Claude, built from the same data.
