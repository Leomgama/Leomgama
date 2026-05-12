# Hi, I'm Leonardo Gama 👋
### Data Analyst | Business Intelligence | SQL • Python • Power BI • Machine Learning
![SQL](https://img.shields.io/badge/SQL-Advanced-blue)
![Power BI](https://img.shields.io/badge/Power%20BI-DAX-yellow)
![Python](https://img.shields.io/badge/Python-Data%20Analysis-3776AB)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--learn-orange)
![R](https://img.shields.io/badge/R-ARIMA%20Forecasting-276DC3)
![Excel](https://img.shields.io/badge/Excel-Analytics-green)
![Google Data Analytics](https://img.shields.io/badge/Google-Data%20Analytics%20Certified-brightgreen)
---
## 👤 About Me
Data Analyst and Business Intelligence professional with a **BBA in Business Management** and a strong foundation in **finance, business analytics, and machine learning**.
I deliver end-to-end analytics solutions using **SQL, Python, Power BI, and Scikit-learn**, with experience across **EDA, ETL, KPI reporting, dashboard development, customer segmentation, churn prediction, geospatial analysis, and time series forecasting**.
My work combines **technical analytics skills** with **business and financial thinking** to translate complex data into clear, actionable insights.
I apply **CRISP-DM methodology** across all projects and document everything here on GitHub.
---
## 🛠️ Tech Stack
### Languages
- **SQL** • **Python** • **DAX** • **M (Power Query)** • **R**
### Python Libraries & ML
- **Pandas** • **NumPy** • **Matplotlib** • **Seaborn**
- **Scikit-learn** (Random Forest, KMeans, Decision Tree, StandardScaler)
- **Folium** • **Altair** • **Streamlit**
- **OpenRouteService API**
### BI & Tools
- **Power BI** • **Power Query** • **SQL Server (SSMS)**
- **Jupyter Notebook** • **VS Code**
- **Git** & **GitHub**
### Core Skills
- EDA • ETL • Churn Prediction • Customer Segmentation • RFM Analysis
- Geospatial Analysis • Pareto Analysis
- Time Series Forecasting (ARIMA) • Business Storytelling
---
## 📂 Featured Projects
### 🎯 Olist RFM Customer Segmentation — Brazilian E-Commerce
**Tools:** Python | Pandas | NumPy | Scikit-learn (KMeans, StandardScaler) | Matplotlib | Seaborn
- Segmented **93,357 unique customers** across **96,477 delivered orders** (R$ 15.4M revenue) into the **11 industry-standard RFM segments** (Champions, Loyal, At Risk, Lost, etc.) for marketing prioritization
- Identified and fixed a **silent schema bug** in the reference methodology — Olist generates a fresh `customer_id` per order, so the actual identity lives in `customer_unique_id`; without that fix, every customer's Frequency collapses to 1
- Computed two scoring methods in parallel (rank-weighted vs. quintile + 11-segment grid) and validated with **KMeans (k=4)** clustering on log-transformed R/F/M
- Quantified **R$ 1.88M of addressable marketing opportunity** (~12% of revenue) across the 11 segments, with conservative per-segment conversion-rate assumptions
- Top plays identified: Potential Loyalist conversion (R$ 634K), Champions retention (R$ 289K), At Risk win-back (R$ 158K)
🔗 [View Repository](https://github.com/Leomgama/OlistRFM)
---
### 👥 AdventureWorks DTC Customer Profitability — AI-Assisted Power BI
**Tools:** Power BI Desktop | DAX | SQL Server (SSMS) | Power BI Modeling MCP | AdventureWorksDW2022
- Built a **four-page Power BI report** (Customer Overview → Demographic Profitability → High-Value Segment → Targeting Recommendations) on **60,398 DTC sales** and **18,484 customers**, including a custom theme JSON for consistent navy-led styling
- Authored **22 DAX measures** organized into 5 analytical themes plus **5 calculated columns** on the customer dim — applied directly to the live model via the Power BI Modeling MCP (XMLA endpoint), no copy-paste
- Identified that the **$40–100K mid-income bracket drives 62% of profit** (vs. only $323K from $150K+), and that the **top 20% of customers generate 66.42% of revenue** with a CLV of **$2,169 (3.3× the overall average)**
- Defined the ideal acquisition target — Bachelor's-educated Professionals/Management in the $40–100K bracket — and recommended a win-back trigger at the 60–90 day silence window to lift repeat rate from **37.1% to 45%**
- Caught two AI-generated bugs in real time (a reserved-word DAX collision and a heavy-compute calculated column) — the analyst still owns correctness
🔗 [View Repository](https://github.com/Leomgama/DTC-Customer-Profitability-Claude)
---
### 🔮 Customer Churn Prediction — B2B Supply Distributor
**Tools:** Python | Pandas | Scikit-learn (Random Forest) | Matplotlib | Seaborn
- Analyzed **11,233 sales records** and **544 customer profiles** from a fictional South Carolina distributor to predict which customers were at risk of churning
- Trained a **Random Forest Classifier** achieving **100% accuracy** on a **109-sample test set**, scoring all active 2025 customers by churn risk level
- Identified **days since last purchase** as the strongest predictor (~20% feature importance) and found **month-to-month customers churn at 2x the rate** of annual contracts
- Delivered 5 targeted retention recommendations including an early-warning flag system for accounts silent **60+ days**
🔗 [View Repository](https://github.com/Leomgama/CustomerChurn)
---
### 🗺️ Customer Geographic Segmentation & Classification
**Tools:** Python | Scikit-learn (KMeans, Decision Tree) | Pandas | Folium | Matplotlib
- Applied **KMeans clustering** to geographically segment **1,000 customers** into **5 commercial divisions** based on latitude & longitude, validated using the Elbow Method
- Trained a **Decision Tree Classifier** on the cluster output achieving **100% accuracy** on **200 test samples** — enabling fully automated real-time classification of new customers
- Visualized all customer divisions on interactive maps using **Folium**
🔗 [View Repository](https://github.com/Leomgama/CustomerClassification)
---
### 📍 Route Change Impact Analysis: Sorocaba vs. Campinas
**Tools:** Python | Pandas | OpenRouteService API | Folium | Jupyter Notebook
- Built a route simulation engine integrating the **OpenRouteService API** to calculate real driving distances and compare delivery scenarios across **6 days**
- Quantified that an emergency branch change increased total weekly route distance from **5,522 km to 10,250 km** — an increase of **+4,728 km (+85.6%)**
- Visualized both route scenarios on interactive maps using Folium and delivered business-focused recommendations on inventory planning and contingency routing
🔗 [View Repository](https://github.com/Leomgama/RouteAnalysis)
---
### 📉 BF LUBS Sales Volume Decline Analysis
**Tools:** Python | Pandas | NumPy | Matplotlib | Seaborn | Jupyter Notebook
- Analyzed **601,836 transactions (2018–2024)** to diagnose a business paradox where revenue grew while sales volume and active customer count both declined
- Applied IQR outlier treatment calibrated against operational context and **Pareto analysis** to identify that one region-market-segment combination drove **28.95% of total volume loss**
- Delivered targeted commercial recovery recommendations prioritized by business impact
🔗 [View Repository](https://github.com/Leomgama/bf-lubs-sales-volume-decline-analysis)
---
### 📈 S&P 500 Financial Performance Analysis (2020–2021)
**Tools:** SQL Server | Power BI (DAX) | R (ARIMA Forecasting)
- Analyzed **~500 S&P 500 companies** post-pandemic using SQL Server, **13 custom DAX measures**, and an **ARIMA forecast model in R** integrated directly inside Power BI
- Identified total revenue doubling from **$5.6T to $13.1T** with net income margin improving from **8% to 11%** across **6 interactive dashboards**
- Found no direct correlation between company size and profitability — business model drives margins more than revenue scale
🔗 [View Repository](https://github.com/Leomgama/sp500-financial-performance-2020-2021)
---
### 📊 U.S. Sales Performance Analysis — AdventureWorks
**Tools:** SQL Server | Power BI | Power Query | DAX
- Built a snowflake schema data model with **20 custom DAX measures** and **3 interactive dashboards** with collapsible navigation menus and custom tooltip pages
- Identified **$9.39M in revenue**, **$3.91M in profit**, and **41.5% average margin** across **5 U.S. regions**
- Pareto analysis confirmed top **27 SKUs** generated **~80% of total revenue**; Accessories (~62.6%) and Mountain Bikes (~45.4%) were top profitability drivers
🔗 [View Repository](https://github.com/Leomgama/US-Sales-Performance-AdventureWorks)
---
## 📚 Certifications
- ✅ Google Data Analytics Professional Certificate
- ✅ SQL for Data Analysis
- ✅ Power BI & Data Analytics
- ✅ Python Fundamentals
- ✅ Python for Data Analysis
---
## 🔗 Connect With Me
- **LinkedIn:** [linkedin.com/in/leonardo-gama-a99648279](https://www.linkedin.com/in/leonardo-gama-a99648279/)
- **Streamlit:** [share.streamlit.io/user/leomgama](https://share.streamlit.io/user/leomgama)
