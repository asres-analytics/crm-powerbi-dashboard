# 📊 Donor CRM Analytics Dashboard

---

##  Overview

This project performs end-to-end CRM data analysis to uncover insights into donor behavior, engagement, and revenue contribution.

The workflow includes:
- Data cleaning and preprocessing using Python (Pandas)
- Feature engineering
- Customer segmentation
- Exploratory data analysis (EDA)
- Preparing data for Power BI dashboard visualization


##  Objectives

- Clean and preprocess CRM donor data  
- Analyze total revenue and donation behavior  
- Identify high-value customers  
- Evaluate engagement impact on donations  
- Segment customers based on contribution  
- Prepare dataset for Power BI dashboard  


##  Dataset Information

###  Dataset Source

The dataset used in this project is sourced from Kaggle:

- [Customer Relationship Management (CRM) Dataset](https://www.kaggle.com/datasets/gaurobsaha/customer-relationship-management-dataset)

###  Key Fields

| Column             | Description                |
|--------------------|----------------------------|
| DonorID            | Unique donor identifier    |
| FirstName          | Donor first name           |
| LastName           | Donor last name            |
| City               | Donor city                 |
| State              | Donor state                |
| LastDonationDate   | Most recent donation date  |
| TotalGifts         | Total number of donations  |
| TotalAmountDonated | Total donation amount      |
| EventParticipation | Event participation status |
| EngagementScore    | Donor engagement score     |

---

## Tools Used

- Python (Pandas, NumPy)
- Matplotlib & Seaborn
- Power BI
- Excel
- Git & GitHub  



##  Data Processing

The dataset was prepared by:

- Removing duplicates  
- Handling missing values  
- Converting date fields to datetime  
- Creating new features:
  - Year  
  - Month  
  - Segment (High / Medium / Low)  


## Analysis Performed

###  Revenue Analysis
- Total revenue generated  
- Overall donation performance  



###  Customer Segmentation

Customers were grouped based on donation value:

| Segment      | Donation Amount     |
|--------------|--------------------|
| High Value   | Above $15,000       |
| Medium Value | $7,000 – $15,000    |
| Low Value    | Below $7,000        |



### Engagement Analysis
- Relationship between engagement score and donation  
- Identification of high-value engaged customers  



### Top Donors Analysis
- Identified top contributors based on total donation  
- Highlighted high-value customers driving revenue  



### Revenue by Segment
- Analyzed contribution of each customer segment  
- Compared revenue distribution across segments  



##  Key Insights

- High-value customers generate the majority of total revenue  
- A small group of customers contributes most of the revenue  
- Higher engagement is associated with higher donation amounts  
- Customer segmentation clearly identifies valuable customer groups  



## Business Impact

This project helps organizations:

- Improve customer retention strategies  
- Identify and target high-value customers  
- Increase fundraising efficiency  
- Make data-driven decisions  
- Enhance customer engagement strategies  



## Dashboard Preview

(Add Power BI screenshots here after dashboard creation)

images/dashboard-overview.png  
images/customer-segmentation.png  
images/engagement-analysis.png  

---

##  Project Structure


```
crm-powerbi-dashboard/
│
├── data/
│   ├── raw/
│   │   └── CRM_Donor_Simulation_Dataset (2).csv
│   │
│   └── processed/
│       └── cleaned_crm_data.csv
│
├── notebooks/
│   └── crm_analysis.ipynb
│
├── dashboard/
│   └── (Power BI files will be added here)
│
├── images/
│   └── (Dashboard screenshots will be added here)
│
├── .gitignore
├── README.md

```

## 👨‍💻 Author
**Asres Gamu Yelia**
### Data Analyst | Power BI Developer | SQL & Excel Specialist

## Connect With Me

[LinkedIn](https://www.linkedin.com/in/asres-analytics)

[Hire me](https://www.upwork.com/freelancers/~013847c2b7252ddb3f)
