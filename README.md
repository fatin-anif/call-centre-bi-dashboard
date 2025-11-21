# call-centre-bi-dashboard
Excel BI project analysing call centre performance, customer experience, and operational metrics.
📊 Call Centre Customer Experience BI Dashboard

Excel • Power Query • Data Model • PivotCharts • DAX-style Measures

🔍 Project Overview

This project analyses call-centre performance and customer experience using a fully interactive BI dashboard built in Microsoft Excel.
It simulates a real operational environment with datasets for Calls, Agents, Customer Feedback, and Workforce Forecasting.

The dashboard provides insights into:

Average Wait Time

Handle Time

Abandon Rate

CSAT (Customer Satisfaction)

Queue-level and Agent-level performance

Forecast vs Actual call volume

🛠 Tools & Techniques Used

Excel Power Query — data cleaning & transformation

Excel Data Model — relationships across 4 tables

Power Pivot Measures — AVERAGE(), DIVIDE(), COUNTROWS() etc.

PivotTables & PivotCharts — KPIs, trend analysis, queue insights

Interactive Slicers — filter by Queue, AgentID, Date, Abandoned

Dashboard Design — clean layout, KPIs, charts, filters

📁 Data Sources (included in repo)

calls.xlsx

agents.xlsx

feedback.xlsx

workforce.xlsx

Final Dashboard .xlsx

These datasets were generated to mimic real call-centre structures.

⭐ Key Measures Created
Avg Wait Time := AVERAGE(Calls[WaitTime])

Avg Handle Time := AVERAGE(Calls[HandleTime])

Abandon Rate :=
DIVIDE(
    CALCULATE(COUNTROWS(Calls), Calls[Abandoned] = "Y"),
    COUNTROWS(Calls)
)

Total Calls := COUNTROWS(Calls)

📈 Dashboard Features
✔ KPIs

Total Calls

Avg Wait Time

Avg Handle Time

Abandon Rate

✔ Visuals

Calls by Queue

Avg Wait Time by Queue

CSAT by Queue

✔ Filters

Queue

AgentID

Abandoned (Y/N)

Date

🎯 Skills Demonstrated

Business Intelligence reporting

Customer experience analytics

Operational performance analysis

Power Query transformation

Data modelling and relationships

KPI creation and storytelling

Dashboard UI/UX design

Excel BI workflow end-to-end

📬 Contact

Feel free to reach out for collaboration or improvement ideas.
