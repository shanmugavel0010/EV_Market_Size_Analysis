🔋 Electric Vehicle Market Size Analysis
Show Image
Show Image
Show Image
Show Image

📌 Objective
Analyzed 1,77,861 EV registration records from Washington State to:

Identify geographic distribution of EV adoption
Understand electric range trends across model years
Forecast future EV registrations using machine learning
Segment EV market by Make, Model, and Vehicle Type


📂 Dataset
DetailInfoSourceWashington State Department of LicensingDataset NameElectric Vehicle Population DataRecords1,77,861 rowsColumns17 featuresLinkdata.wa.gov

🛠️ Tools & Libraries Used
ToolPurposePython 3.8+Core programming languagePandasData manipulation & cleaningMatplotlibData visualizationSeabornStatistical visualizations & heatmapsSklearnKMeans clustering & Linear RegressionNumPyNumerical computationsJupyter NotebookInteractive development environment

📁 Project Structure
EV_Market_Analysis/
│
├── 📓 EV_Analysis.ipynb          # Main analysis notebook
├── 📊 Market_Size_Analyze.xlsx   # Raw dataset
├── 📄 README.md                  # Project documentation
│
├── 📁 DASHBOARD/
│   ├── charts/
│   │   ├── ev_registrations_by_year.png
│   │   ├── electric_range_histogram.png
│   │   ├── electric_range_boxplot.png
│   │   ├── county_heatmap.png
│   │   ├── city_heatmap.png
│   │   ├── ev_clustering.png
│   │   ├── make_bar_chart.png
│   │   ├── model_bar_chart.png
│   │   ├── ev_type_pie_chart.png
│   │   ├── cafv_pie_chart.png
│   │   ├── correlation_matrix.png
│   │   └── ev_forecast.png
│   └── reports/
│       └── EV_Market_Report.docx

🧹 Data Cleaning Steps
ProblemSolution⚡ Electric Range = 0 (91,950 rows)Filled with separate BEV & PHEV medians💰 Base MSRP = 0 (98% missing)Dropped the column📍 Vehicle Location (POINT format)Split into Longitude & Latitude🏙️ Blank City/County (5 rows)Dropped rows (0.002% of data)🏛️ Legislative District (389 blanks)Dropped rows (0.2% of data)

📊 Analysis Performed
1️⃣ Descriptive Analysis

Summary statistics using describe()
Distribution of Electric Range (Histogram & Box Plot)
BEV Median Range: 215 miles
PHEV Median Range: 28 miles

2️⃣ Time-Series Analysis

EV registrations grouped by Model Year
Massive growth observed from 2010 to 2023
Peak registrations in 2023 (~57,000 EVs)

3️⃣ Geographical Analysis

County heatmap: King County leads with 92,740 EVs
City heatmap: Seattle leads with 29,447 EVs
KMeans Clustering (K=3) identified EV adoption hotspots

4️⃣ Segmentation Analysis

Top Make: Tesla (80,000+ EVs)
Top Model: Model Y (35,921 EVs)
EV Type split: BEV = 78.3%, PHEV = 21.7%
CAFV Eligibility: 37.3% eligible for clean fuel benefits

5️⃣ Electric Range Analysis

Range improved significantly after 2018
No correlation between location (Lat/Long) and range
Model Year vs Range correlation: 0.34

6️⃣ Correlation Analysis

Correlation matrix for all numerical variables
Strongest relationship: Electric Range vs Model Year (0.34)
Location has no significant effect on range

7️⃣ Forecasting

Linear Regression model trained on historical data
Predicted EV registrations till 2028

YearPredicted EVs202419,715202520,678202621,641202722,605202823,568

🔑 Key Findings

🏆 Tesla dominates the EV market with 80,000+ registrations
🏙️ Seattle & King County are the biggest EV hotspots
📈 EV market has grown massively since 2010
🔋 78.3% of EVs are fully electric (BEV)
📍 Location does NOT affect electric range
📅 Newer cars have better range (correlation = 0.34)


🚀 How To Run
bash# Step 1 - Clone the repository
git clone https://github.com/yourusername/EV_Market_Analysis.git

# Step 2 - Install required libraries
pip install pandas matplotlib seaborn scikit-learn numpy openpyxl jupyter

# Step 3 - Open Jupyter Notebook
jupyter notebook EV_Analysis.ipynb

📈 Sample Visualizations
ChartInsight📊 EV Registrations by YearMassive growth after 2010🗺️ County HeatmapKing County dominates🥧 EV Type Pie ChartBEV = 78.3%🔮 Forecast ChartSteady growth till 2028

👤 Author
Your Name

📧 Email: yourname@email.com
💼 LinkedIn: linkedin.com/in/yourname
🐙 GitHub: github.com/yourusername


📄 License
This project is licensed under the MIT License


🧸 "Data tells a story — you just need to know how to read it!" 📊
