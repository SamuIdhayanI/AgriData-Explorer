# AgriData Explorer: A Data Visualization Platform for Indian Agriculture

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


### 1️⃣ Home Screen
Central hub with navigation links to all insights pages.
![image](https://github.com/user-attachments/assets/7de7113a-29e6-4e78-8017-5edaeaa4ce31)


### 2️⃣ National Crop Production Overview  
Macro-level view of India’s total production, area, and yield.
![image](https://github.com/user-attachments/assets/b4b31512-13b6-4334-b9a2-d8aa1bd49ab2)


### 3️⃣ Crop-Specific Trends Over Time  
Explore production and yield trends for each major crop.
![image](https://github.com/user-attachments/assets/0fd7603f-5809-4362-97b1-740225739e43)


### 4️⃣ Regional and District-Level Insights  
District-wise breakdown and comparisons for selected crops.
![image](https://github.com/user-attachments/assets/26e2dfed-8731-484e-97d3-a921fe26063e)

### 5️⃣ Yield and Efficiency Analysis  
Comparison of crop yields and cultivation efficiency.
![image](https://github.com/user-attachments/assets/58de4ec8-2d65-4ebc-8df2-acf36ffa3759)

### 6️⃣ Growth and Performance Analytics  
Focus on recent changes in area and production across years.
![image](https://github.com/user-attachments/assets/b5c47339-b66f-4e4a-9cff-2512a5a60546)

### 7️⃣ Crop-Specific Insights  
Dedicated views for key crops: Rice, Wheat, Oilseeds, Groundnut, Sugarcane, Sunflower.
![image](https://github.com/user-attachments/assets/79514348-90fa-4ef9-8eea-fd2fef15aeb6)

> 📌 All dashboards include **customized tooltips**, **icons**, and **themed visuals** to enhance clarity and user experience.
> ![image](https://github.com/user-attachments/assets/84d238e3-c0c6-404e-909f-d87e9a502b91)


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
