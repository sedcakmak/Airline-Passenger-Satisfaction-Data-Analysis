# ✈️ Airline Passenger Satisfaction Data Analysis

This project is developed as the first final case study for the **Data Analysis Bootcamp** organized by **[Patika.dev](https://www.patika.dev) & [Kız Başına](https://www.kizbasina.com/)**.

## 📌 Project Description

Using the Airline Passenger Satisfaction dataset from [Kaggle](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction/data), this project analyzes passenger demographics, service ratings, delay patterns, and satisfaction levels through statistical summaries, outlier analysis, missing data handling, and visualizations.

## 🎯 Project Objectives

- Dataset selection & setup  
- Statistical summary  
- Missing data analysis  
- Outlier detection  
- Visualization of key variables  

## 🔍 Dataset Info

**Source:** Kaggle  
**Files Used:** `train.csv`, `test.csv`  
**Total Records:** Combined from both train and test sets  

## 🛠️ Technologies Used
The analysis was conducted using Python with pandas for data manipulation, matplotlib and seaborn for visualization, and kagglehub for dataset management.

---

## 🔍 Analysis Results

### Data Quality and Missing Values

The dataset included two unnecessary columns (Unnamed: 0 and id) which were dropped from the analysis. It also showed minimal missing values, found only in the "Arrival Delay in Minutes" column. These missing values were successfully handled using median imputation, with the median value of 0.0 minutes indicating that at least 50% of flights had no arrival delay.

### Outlier Detection

Using the Interquartile Range (IQR) method, I analyzed four key variables for outliers. Age data showed no outliers, indicating reliable demographic data collection. Flight distance revealed 2,855 outliers, but these represent legitimate long-haul international flights rather than data errors.
However, delay data revealed significant operational challenges. Departure delays contained 18,098 outliers while arrival delays had 17,492 outliers. The most extreme cases were concerning, with the longest departure delay reaching 1,592 minutes (26.5 hours) and the longest arrival delay at 1,584 minutes (26.4 hours). I have also used Boxplot to further understand the outliers in delays.

### 🧠 Key Findings

The analysis revealed a fairly balanced gender distribution with the majority of passengers being adults and small percentages under 18 and over 65. Service ratings were mostly within the expected 1–5 range, though delay fields contained significant outliers suggesting operational challenges. Overall satisfaction levels lean slightly positive, with Business class passengers consistently showing higher satisfaction rates compared to Economy and Eco Plus classes across all service categories. Most importantly, the data showed a moderate correlation between departure and arrival delays, indicating that when flights leave late, they tend to arrive late as well, suggesting that addressing departure timing issues could significantly improve overall flight performance.

## 📊 Sample Visualizations

Visualizations include:
- Gender distribution  
- Age histogram  
- Customer satisfaction pie chart  
- Satisfaction by class bar plot  
- Service rating heatmap  
- Delay scatter plot  


