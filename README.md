# IT Asset & Cost Management in Excel  

##  Overview  
This project demonstrates **Excel data analysis skills** by managing and analyzing **IT assets**, focusing on:  

- **Cost Management** – Analyzing purchase, maintenance, and license fees  
- **Compliance & Status Tracking** – Identifying non-compliant and expired assets  
- **Data Cleaning & Transformation** – Formatting, removing duplicates, and handling missing values  
- **Advanced Excel Functions & Formulas** – **IF, COUNTIF, SUMIFS, AVERAGEIF**  
- **Data Visualization** – Creating **Pivot Tables, Charts, and Insights**  

🔹 **Goal:** Showcase **Excel proficiency**   

---

## 📂 Folder Structure  

📂 IT_Asset_Cost_Management_in_Excel
│-- 📂 datasets # Contains raw and cleaned Excel datasets
│-- 📂 images # Contains visualized charts and analysis images
│-- 📂 notebooks # Jupyter Notebook used to generate the dataset
│-- 📄 README.md # Project documentation


---

## The Dataset  

Since this project **does not use real-world data**, I **randomly generated a simulated dataset** using **Python (Pandas & NumPy)**.  
The dataset consists of **100 IT assets** with key attributes like:  

📄 **Dataset Generation Notebook:** [`Generated_data_randomly.ipynb`](notebooks/Generated_data_randomly.ipynb)

| Column Name        | Description |
|-------------------|-------------|
| **Asset_ID**       | Unique identifier for each IT asset |
| **Asset_Type**     | Category of asset (Laptop, Server, Software, etc.) |
| **Vendor**         | The company providing the asset (Dell, AWS, Oracle, etc.) |
| **Purchase_Date**  | Date when the asset was purchased |
| **Status**         | Current status of the asset (Active, Expired, Under Maintenance, etc.) |
| **Purchase_Cost**  | Initial purchase cost of the asset |
| **Maintenance_Cost** | Annual maintenance expenses |
| **License_Fee**    | Software licensing cost (if applicable) |
| **Last_Used_Date** | Last recorded usage of the asset |
| **Compliance_Status** | Indicates if the asset is **Compliant** or **Non-Compliant** |

📄 **Dataset Files:**  
✔️ [`IT_Asset_Management.xlsx`](datasets/IT_Asset_Management.xlsx) – **Raw dataset (Generated with Python)**  
✔️ [`Cleaned_IT_Asset_Management.xlsx`](datasets/Cleaned_IT_Asset_Management.xlsx) – **Cleaned & Transformed dataset**  

---

## 🛠 Data Cleaning & Transformation  

### **1️⃣ Data Cleaning in Excel**
To ensure **data integrity**, I performed:  

✔️ **Fixing Date Formatting** – Standardized **Purchase_Date** and **Last_Used_Date**  
✔️ **Handling Missing Values** – Used `=COUNTBLANK(F:F)` to check missing values  
✔️ **Removing Duplicates** – Used **Remove Duplicates** feature  
✔️ **Standardizing Status Column** – Ensured consistent values across **Active, Expired, Inactive, etc.**  

📄 **Cleaned dataset stored in:** [`Cleaned_IT_Asset_Management.xlsx`](datasets/Cleaned_IT_Asset_Management.xlsx)  

---

## Excel Functions & Analysis  

### **2️⃣ Excel Functions Used**
To perform the analysis, I used the following **Excel functions**:  

✔️ `=IF(E2="Expired", "Yes", "No")` → **Flagging assets that need replacement**  
✔️ `=COUNTIF(J:J, "Non-Compliant")` → **Counting non-compliant assets**  
✔️ `=SUMIFS(F:F, B:B, "Laptop")` → **Summing purchase costs per asset type**  
✔️ `=AVERAGEIF(C:C, "Dell", G:G)` → **Calculating average maintenance cost per vendor**  
✔️ `=COUNTIF(E:E, "Under Maintenance")` → **Counting assets under maintenance**  

---

## Data Visualizations  

### **3️⃣ Pivot Tables & Charts**
To better **understand IT asset costs and compliance**, I created various **charts** and **pivot tables**.  

📄 **Pivot Table Example:** Vendors' Total Costs  

| Vendor   | Maintenance Cost | Purchase Cost | License Fee |
|----------|----------------|---------------|------------|
| **AWS**  | 17,938.65 | 93,055.48 | 36,145.75 |
| **Cisco** | 9,566.44 | 83,206.56 | 31,223.41 |
| **Dell**  | 9,194.48 | 43,537.26 | 29,453.04 |
| **Microsoft** | 15,001.09 | 50,995.8 | 29,503.25 |
| **Oracle** | 15,198.26 | 73,063.95 | 34,400.70 |

---

#### Key Findings from Data Analysis  

**1️⃣ Asset Distribution**  
- **Databases (21%)** make up the largest asset category.  
- **Laptops (11%)** and **Networking Equipment (13%)** are smaller but significant categories.  

![Asset Distribution by Type](images/Asset%20Distribution%20by%20Type.png)  

**2️⃣ Compliance Status of Assets**  
- **45% of assets are non-compliant** and might require intervention.  

![Non-Compliant vs. Compliant Assets](images/Non-Compliant%20vs.%20Compliant%20Assets.png)  

**3️⃣ Asset Lifecycle Status**  
- **31% of assets are under maintenance**, while **27% are expired**.  

![Proportion of Asset Status](images/Proportion%20of%20Expired,%20Inactive,%20Active,%20and%20Under%20Maintenance%20assets.png)  

**4️⃣ Maintenance Cost Per Vendor**  
- **HP and Microsoft have the highest average maintenance costs**, while **Cisco has the lowest**.  

![Average Maintenance Cost](images/Average%20Maintenance%20Cost%20per%20Vendor.png)  

**5️⃣ Total Purchase Cost Per Asset Type**  
- **Database assets have the highest total purchase cost (~$102K).**  

![Total Purchase Cost per Asset Type](images/Total%20Purchase%20Cost%20per%20Asset%20Type.png)  

**6️⃣ Cost Breakdown by Vendor**  
- AWS, Microsoft, and Oracle have the highest **overall IT costs**.  

![Vendor Costs](images/Vendors%20Costs.png)  

---

## Conclusion, Limitations & Future Improvements  

### **Conclusion**  

This project successfully demonstrates **IT Asset Management using Excel**, showcasing:  
✔️ **Data Cleaning & Transformation** – Ensuring data integrity  
✔️ **Formula-Based Analysis** – Using Excel functions to extract insights  
✔️ **Data Visualization** – Creating pivot tables & charts for cost & compliance tracking  



### **Limitations**  

🔹 **Simulated Data** – Since the dataset is randomly generated, it does not reflect **real-world business challenges**.  
🔹 **Lack of Real Trends** – No seasonality, vendor-specific pricing, or market fluctuations.  
 



### **Future Improvements**  

✔️ **Develop an Interactive Dashboard** – Use **Power BI** or **Tableau** to improve visual analysis.  
✔️ **Use Real-World Data** – Incorporate actual IT asset data for realistic insights.  
✔️ **Expand Analysis** – Add **asset depreciation calculations** and **lifecycle forecasting**.  
✔️ **Automate Reporting** – Use **Python or VBA** to generate reports dynamically.  
✔️ **Integrate Cost Optimization** – Identify cost-saving opportunities in IT asset management.  


---

## 🛠 **Technologies Used**  

- **Excel** – Data cleaning, transformation, and visualization  
- **Python (Pandas, NumPy)** – Data simulation for creating realistic IT assets  
- **Excel Functions** – `IF`, `COUNTIF`, `SUMIFS`, `AVERAGEIF`, `Pivot Tables`  
- **Charts & Pivot Tables** – For visualizing key trends in IT asset costs  

---

## 📬 **Contact & Connect**  
📩 [Email Me](mailto:manoskonstantinos960@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/konstantinosmanos)  
🖥 [GitHub](https://github.com/konstantinosmanos)  

🚀 **Like this project? Give it a ⭐ on GitHub!**  
