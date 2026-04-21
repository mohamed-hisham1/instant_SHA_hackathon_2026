# 🚗Car Sales Analytics Dashboard. — Car Sales Intelligence

> End-to-end data analysis solution built for the **Instant SHA Hackathon 2026** — covering data preprocessing, exploratory analysis, feature engineering, and an interactive Streamlit dashboard.

---

## 📌 Project Overview

**AutoPulse** is a complete data analysis pipeline applied to a used car sales dataset. The goal was to extract actionable business insights across pricing, market trends, seller behavior, and geographic distribution — delivered through both structured notebooks and a polished interactive dashboard.

---

## 🗂️ Repository Structure

```
instant_SHA_hackathon_2026/
│
├── 1_preprocessing.ipynb        # Data cleaning & preparation
├── 2_Complete_Analysis.ipynb    # Full exploratory data analysis (EDA)
├── 3_feature_engineering.ipynb  # Feature creation & transformation
│
├── cleaned_data.csv             # Processed dataset output
├── dashboard.py                 # Streamlit interactive dashboard (AutoPulse)
└── requirements.txt             # Project dependencies
```

---

## 🔍 Analysis Pipeline

### 1. Preprocessing (`1_preprocessing.ipynb`)
- Handling missing values and duplicates
- Type casting and schema normalization
- Outlier detection and treatment

### 2. Exploratory Data Analysis (`2_Complete_Analysis.ipynb`)
- Univariate and bivariate analysis
- Distribution of selling prices, odometer readings, and condition scores
- Correlation analysis between key numeric features

### 3. Feature Engineering (`3_feature_engineering.ipynb`)
- Derived features: `Gross` (SellingPrice − MMR), `GrossMarginPct`, `Underpriced` flag
- Categorical encoding and aggregation features
- Data prepared for downstream modeling or reporting

---

## 📊 Dashboard

An interactive **Streamlit + Plotly** dashboard with 7 analytical tabs:

| Tab | Focus |
|-----|-------|
| 📅 Time | Monthly/yearly revenue trends, sales volume over time |
| 🏷️ Brand & Market | Top makes by volume and price, make-model heatmap |
| 🔩 Trim & Body | Body type distribution, trim popularity, transmission breakdown |
| 💰 Price & Value | Price distribution, MMR vs selling price scatter, underpriced cars |
| 🔧 Condition & Usage | Condition impact on price, odometer distribution and correlation |
| 🏪 Sellers | Top sellers by volume, avg price, and gross margin |
| 🌍 Geography | US state-level choropleth maps for volume and avg price |

**KPI Cards at a glance:** Total Revenue · Avg Selling Price · Avg Gross vs MMR · Underpriced % · Top Make

---
## 📈 Power BI Dashboards

![Dashboard 1](dashboards/Dashboard1.jpg)
![Dashboard 2](dashboards/Dashboard2.jpg)
![Dashboard 3](dashboards/Dashboard3.jpg)
## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Analysis | Python, Pandas, NumPy, Scikit-learn |
| Visualization | Matplotlib, Seaborn, Plotly |
| Dashboard | Streamlit |
| Environment | Jupyter Notebook |

---

## ⚡ Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/mohamed-hisham1/instant_SHA_hackathon_2026.git
cd instant_SHA_hackathon_2026
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the notebooks
Open the notebooks in order using Jupyter:
```bash
jupyter notebook
```

### 4. Launch the dashboard
```bash
streamlit run dashboard.py
```
> Make sure `cleaned_data.csv` is in the same directory as `dashboard.py`.

---

## 📦 Requirements

```
streamlit==1.32.0
pandas==2.2.1
numpy==1.26.4
scikit-learn==1.4.1.post1
matplotlib==3.8.3
seaborn==0.13.2
```

---

## 👤 Author

**Abdelrahman Ibrahim Abdelrahman**  
**Mohamed Hisham Hussain**  
**Nada Rashad Montaser El-Nager**
**Mostafa Sadeq**
---

*Built for Instant SHA Hackathon 2026*
