# **New Jersey Real Estate Property Analysis & Mapping Tool**
### **Capstone Project - Machine Learning Engineering Bootcamp**

📍 **Author:** Tony Clark  
📅 **Date:** *2/7/2025*  
📂 **Repository:** [GitHub Repo Link(https://github.com/TJC1996/NJ-Real-Estate/)

---

## **📌 Project Overview**
This project focuses on **analyzing, cleaning, and visualizing** commercial real estate transactions in **New Jersey**. The tool integrates **geospatial mapping, data wrangling, and interactive visualization** to provide insights into **property sales trends, buyer/seller transactions, and valuation metrics.**

The project covers:
- **Data Wrangling & Cleaning:** Handling missing values, standardizing formats, and feature engineering.
- **Exploratory Data Analysis (EDA):** Distribution analysis, price trends, and outlier detection.
- **Interactive Visualization:** Folium-based **geospatial property mapping**.
- **Real Estate Insights:** Identifying **hotspots for investment** and **historical sale trends**.

---

## **🛠️ Technologies Used**
- **Python Libraries:**
  - `pandas` – Data manipulation
  - `numpy` – Numerical operations
  - `geopandas` – Geospatial data processing
  - `folium` – Interactive map visualizations
  - `matplotlib` & `seaborn` – Data visualization
  - `contextily` – Basemap integration for geospatial plots
- **Data Sources:**
  - NJ County Public Property Records (CSV Format)

---

## **📊 Dataset Description**
The dataset contains **commercial property transactions** in New Jersey, with features such as:
| **Column Name**    | **Description** |
|--------------------|---------------|
| `Property Location` | Address of the property |
| `Sale Price` | Price at which the property was sold |
| `Sale Date` | Date of sale transaction |
| `Latitude/Longitude` | Geographic coordinates |
| `Owner's Name` | Name of the property owner |
| `Seller Name` | Previous owner (Derived Feature) |
| `Buyer Name` | Current owner (Derived Feature) |
| `Total Assmnt` | Assessed property value |
| `Acreage` | Size of the property in acres |
| `Sq. Ft.` | Building square footage |

---

## **📈 Data Cleaning & Processing**
**Steps taken to clean the dataset:**
1. **Handled missing values** in critical fields (`Sale Price`, `Latitude/Longitude`, `Total Assmnt`).
2. **Converted date fields** (`Sale Date`) into standard datetime format.
3. **Filtered invalid data points** (e.g., removed sale prices ≤ 0).
4. **Created unique property IDs** to track multiple transactions.
5. **Derived new features:**
   - `Seller Name` & `Buyer Name` extracted from ownership records.
   - `Lot Price per Acre` and `Building Price per Sq.Ft.` calculated.

---

## **📍 Geospatial Visualization**
🔹 **Interactive Property Map** *(Using Folium)*
- Visualizes **property sales** in NJ with **color-coded markers**:
  - 🔴 **High-value properties**: Over **$10M**
  - 🟢 **Mid-range**: $2.5M - $10M
  - 🔵 **Affordable**: Below $500K
- Clickable **popups** display **property sale details, buyer/seller history, and assessed values**.

🔹 **Property Sale Trends by Municipality** *(Using Seaborn & Matplotlib)*
- **Boxplot analysis** of sale prices across **top municipalities**.
- Identifies **high-value locations vs. undervalued regions**.

🔹 **Correlation Heatmap**
- Shows how factors like **square footage, acreage, and assessed value** impact **sale price**.

---

## **💻 Installation & Setup**
To run this project, follow these steps:

1️⃣ **Clone the Repository**
```bash
git clone https://github.com/your-repo
cd your-repo
```

2️⃣ **Install Dependencies**
```bash
pip install pandas numpy geopandas folium matplotlib seaborn contextily
```

3️⃣ **Run Jupyter Notebook**
```bash
jupyter notebook
```
- Open **`real_estate_analysis.ipynb`** and execute the code.

---

## **📊 Sample Visualizations**
### **1️⃣ Sale Price Distribution**
![](example_sale_price_histogram.png)

### **2️⃣ Property Location Map**
![](example_folium_map.png)

### **3️⃣ Heatmap of Missing Data**
![](example_missing_data_heatmap.png)

---

## **🔮 Business Insights & Key Findings**
**1️⃣ Property Valuation Trends**
- Properties in **Monmouth County & Ocean County** show the **highest median sale prices**.
- Commercial properties near **coastal areas** tend to have **higher valuations**.

**2️⃣ Buyer/Seller Behavior**
- Repeated transactions on the same `PropertyID` suggest **flipping activity** in certain areas.
- Certain **investment firms appear multiple times** in transactions.

**3️⃣ Market Opportunities**
- Comparing **sale price vs. assessed value**, certain municipalities have **undervalued properties** worth investigating.

---

## **🚀 Future Enhancements**
✅ **Automate Data Collection** via **real estate APIs (Zillow, Redfin, Realtor.com).**  
✅ **Build a Machine Learning Model** to **predict future property prices** based on historical trends.  
✅ **Integrate Property Tax Analysis** for investment insights.  

---

## **📜 Acknowledgments**
- Special thanks to **Ronnie Schrader and my grandfather** for their insights on NJ commercial real estate.  
- Data sourced from **NJ County Property Records**.  

---

## **📞 Contact**
For inquiries or collaboration:
📩 **Email:** *(Your email here)*  
🐍 **GitHub:** [Your GitHub Profile](https://github.com/your-profile)

---

### ✅ **Final Checklist Before Submission**
- [x] Upload all **Jupyter Notebooks** to GitHub 📂  
- [x] Ensure **README.md** is structured & informative 📝  
- [x] Test all **code cells** before submission 🚀  
- [x] Verify **data visualizations & insights** align with findings 📊  
- [x] Include **sample output images (if applicable)** 📸  

---
