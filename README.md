# Customer Acquisition Cost Analysis

## 📌 Project Overview
This project analyzes **Customer Acquisition Cost (CAC)** using a dataset containing marketing spend and new customer acquisition data. The goal is to evaluate the efficiency of different marketing channels and optimize marketing strategies.

## 📂 Dataset Information
The dataset contains the following columns:
- **Customer_ID**: Unique identifier for customers
- **Marketing_Channel**: The marketing channel used (Email Marketing, Online Ads, Social Media, etc.)
- **Marketing_Spend**: Amount spent on marketing
- **New_Customers**: Number of new customers acquired

## 🛠️ Steps & Analysis
### 1️⃣ Data Loading & Exploration
- Load the dataset using `pandas`
- Display dataset info and first few records

### 2️⃣ Customer Acquisition Cost (CAC) Calculation
- CAC is calculated as:
  ```python
  data['CAC'] = data['Marketing_Spend'] / data['New_Customers']
  ```
- A **bar chart** visualizes CAC by marketing channel.

### 3️⃣ Relationship Between New Customers & CAC
- A **scatter plot** with a trendline examines how new customers influence CAC.

### 4️⃣ Summary Statistics
- **Descriptive statistics** for CAC across different marketing channels.

### 5️⃣ Conversion Rate Analysis
- Calculate **Conversion Rate**:
  ```python
  data['Conversion_Rate'] = (data['New_Customers'] / data['Marketing_Spend']) * 100
  ```
- A **bar chart** displays conversion rates by marketing channel.

### 6️⃣ Break-Even Customer Calculation
- Compute **Break-Even Customers**:
  ```python
  data['Break_Even_Customers'] = data['Marketing_Spend'] / data['CAC']
  ```
- Compare **actual customers acquired** vs. **break-even customers** with a grouped bar chart.

## 📊 Visualizations
The project includes interactive **Plotly** visualizations:
- 📌 **Bar Chart** → CAC by Marketing Channel
- 📌 **Scatter Plot** → New Customers vs. CAC (with trendline)
- 📌 **Bar Chart** → Conversion Rates by Marketing Channel
- 📌 **Bar Chart** → Break-Even Customers by Marketing Channel
- 📌 **Grouped Bar Chart** → Actual vs. Break-Even Customers

## 🔍 Key Insights
✅ **Social Media** has the lowest CAC, making it the most cost-effective channel.
✅ A **negative correlation** between new customers and CAC indicates improved efficiency with increased customer acquisition.
✅ **Online Ads** have the highest conversion rates.
✅ The actual customers acquired **match break-even customers**, validating the success of the marketing campaign.

## 💾 Dependencies
To run this project, install the required libraries:
```sh
pip install pandas plotly
```

## 🚀 How to Run
1️⃣ Clone this repository:
```sh
git clone <repository_url>
cd <repository_folder>
```
2️⃣ Run the script:
```sh
python script.py
```

## 📜 License
This project is open-source and available under the **MIT License**.

---
📌 *Feel free to contribute or report any issues!*

