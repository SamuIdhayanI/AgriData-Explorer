# 🇮🇳 AgriData Explorer: A Data Visualization Platform for Indian Agriculture

## 🌾 Overview

India’s agricultural sector is vital to the country's economy and sustains millions of livelihoods. However, stakeholders such as farmers, policymakers, and researchers struggle with fragmented, inaccessible agricultural data. This project aims to bridge that gap by building a comprehensive data visualization platform that integrates district-level crop production data from across India.

Using Python (for EDA and preprocessing), SQL (for data storage and querying), and Power BI (for interactive dashboards), this project provides visual insights into crop area, production, and yield across various regions. It is intended to support:
- **Farmers** in making informed crop selection decisions.
- **Policymakers** in identifying low-productivity zones and allocating resources effectively.
- **Researchers** in studying long-term agricultural trends and innovations.

## 📊 Dataset

**Source**: ICRISAT – District Level Agricultural Data  
**Primary File**: `ADE_source_data.csv`  

This dataset contains district-level statistics on crop area, production, and yield for key Indian crops like Rice, Wheat, Oilseeds, Cotton, Sugarcane, and more. Data fields include:

- **Geographic Fields**: State Code, State Name, District Code, District Name, Year
- **Crop Metrics**: Area (1000 ha), Production (1000 tons), Yield (kg/ha)
- **Crops Included**: Rice, Wheat, Maize, Groundnut, Sugarcane, Cotton, Oilseeds, Pulses, Fruits, Vegetables, etc.

Cleaned data is saved in `cleaned_agriculture_data.csv`, and is ready for SQL insertion and dashboard integration.

## 🧱 Project Structure

```
├── data/
│   ├── ADE_source_data.csv               # Raw dataset
│   ├── cleaned_agriculture_data.csv      # Cleaned dataset
│   ├── IndiaShape.json                   # GeoJSON file for Power BI map visualizations
│   └── Theme.json                        # Custom Power BI theme
│
├── python/
│   ├── Data_Prep.ipynb                   # Data cleaning and preprocessing
│   ├── EDA.ipynb                         # EDA using matplotlib & seaborn
│   └── SQL.ipynb                         # Store & query dataset using SQL
│
├── ui/
│   ├── backgrounds/                      # Power BI dashboard background images
│   └── icons/                            # Custom icons used in Power BI visuals
│
├── AgriDataExp.pbix                      # Power BI file with all dashboards
└── README.md
```

## ⚙️ Tech Stack

| Tool       | Purpose                             |
|------------|-------------------------------------|
| **Python** | Data cleaning, transformation, EDA  |
| **Pandas** | Data wrangling                      |
| **SQL**    | Data storage and querying           |
| **Matplotlib & Seaborn** | Visual exploration      |
| **Power BI**| Dashboard and storytelling          |

## 📈 Power BI Dashboard Pages

### 1️⃣ Home Screen
Central hub with navigation links to all insights pages.

![Home Screen](screenshots/home.png)

### 2️⃣ National Crop Production Overview  
Macro-level view of India’s total production, area, and yield.

![National Overview](screenshots/national_overview.png)

### 3️⃣ Crop-Specific Trends Over Time  
Explore production and yield trends for each major crop.

![Crop Trends](screenshots/crop_trends.png)

### 4️⃣ Regional and District-Level Insights  
District-wise breakdown and comparisons for selected crops.

![District Insights](screenshots/regional_district.png)

### 5️⃣ Yield and Efficiency Analysis  
Comparison of crop yields and cultivation efficiency.

![Yield Analysis](screenshots/yield_efficiency.png)

### 6️⃣ Growth and Performance Analytics  
Focus on recent changes in area and production across years.

![Growth Performance](screenshots/growth_performance.png)

### 7️⃣ Crop-Specific Insights  
Dedicated views for key crops: Rice, Wheat, Oilseeds, Groundnut, Sugarcane, Sunflower.

![Crop Specific](screenshots/crop_specific.png)

> 📌 All dashboards include **customized tooltips**, **icons**, and **themed visuals** to enhance clarity and user experience.

## 🚀 Getting Started

### 🔧 Prerequisites
- Python 3.x
- Power BI Desktop
- MySQL or SQLite (for SQL notebook)

### 📦 Installation & Usage

1. **Clone the repository**:
```bash
git clone https://github.com/SamuIdhayanI/AgriData-Explorer.git
```

2. **Data Preprocessing (Python)**:
   - Open `python/Data_Prep.ipynb` to clean and export the dataset.
   - Output: `cleaned_agriculture_data.csv`

3. **Run EDA**:
   - Open `python/EDA.ipynb` for visualizations using matplotlib/seaborn.

4. **SQL Queries**:
   - Use `python/SQL.ipynb` to store and query data from SQL.

5. **Open Power BI Dashboards**:
   - Open `AgriDataExp.pbix` in Power BI Desktop.
   - Ensure the `cleaned_agriculture_data.csv` path is valid and maps are loaded using `IndiaShape.json`.
   - Apply theme using `Theme.json` (Power BI > View > Browse for Themes).

## 📫 Contact

For questions or contributions, feel free to reach out via GitHub issues or email at:  
📧 **samidhayani@gmail.com**
