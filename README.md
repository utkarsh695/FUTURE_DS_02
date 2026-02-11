📊 Customer Churn Analysis & Retention Dashboard (Power BI)
    📌 Project Overview

        This project analyzes customer churn data to help business teams understand:

        Why customers are leaving the platform

        Which customer segments are most likely to churn

        How long customers typically stay active

        What actions can improve customer retention

        The analysis is performed using Power BI, with interactive dashboards and business-focused insights.

🎯 Business Objectives

       The dashboard aims to:

       Analyze churn rates and retention trends

       Identify high-risk customer segments

       Perform customer cohort analysis

       Examine customer lifetime patterns

       Determine key churn drivers and retention factors

       Provide actionable business recommendations

📂 Dataset Information

      The dataset contains customer subscription information including:

      Demographics (Gender, Senior Citizen, Partner, Dependents)

      Account Information (Tenure, Contract Type, Payment Method)

      Services Used (Internet Service, Streaming, Tech Support, etc.)

      Billing Data (Monthly Charges, Total Charges)

      Churn Status (Yes/No)

      Total Records: ~7,000 customers

🧹 Data Cleaning & Preparation

      The following preprocessing steps were performed in Power BI (Power Query):

      Converted TotalCharges to numeric format

      Removed null or invalid records

      Standardized categorical fields (Yes/No consistency)

   Created tenure-based cohort groups:

    0–1 Year

    1–2 Years

    2–4 Years

    4+ Years

📊 Dashboard Structure
🔹 Page 1: Executive Overview

    Total Customers

    Churn Rate

    Retention Rate

    Average Tenure

    Overall churn distribution

🔹 Page 2: Churn Drivers

    Churn Rate by Contract Type

    Churn Rate by Internet Service

    Churn Rate by Payment Method

🔹 Page 3: Customer Segments & Cohorts

    Churn by Tenure Group

    Churn by Senior Citizen
    Monthly Charges vs Churn

    Interactive slicers for segmentation

🔹 Page 4: Customer Lifetime & Retention Insights

    High-risk customer profile summary

📈 Key Insights
    Why Are Customers Leaving?

    Month-to-month contracts have the highest churn rate

    Fiber optic customers churn more frequently

    Customers using electronic check payments show higher churn

    Early-tenure customers (first 12 months) are most vulnerable

  Which Customers Are Most Likely to Churn?

    Short-term contract users

    High monthly charge customers

    Early-stage subscribers

    Customers without long-term commitment

    How Long Do Customers Stay?

    Most churn occurs within the first year

    Customers staying beyond 24 months have significantly lower churn probability

    Customer Lifetime Patterns

    Long-term contracts generate higher lifetime value

    Early churn results in major revenue loss

🧮 Key DAX Measures Used
   Total Customers = COUNTROWS(churn)

   Churned Customers =
   CALCULATE(COUNTROWS(churn), churn[Churn] = "Yes")

   Churn Rate =
   DIVIDE([Churned Customers], [Total Customers], 0)

   Retention Rate = 1 - [Churn Rate]

   Average Tenure = AVERAGE(churn[tenure])

   Estimated CLV =
   AVERAGEX(
       churn,
       churn[MonthlyCharges] * churn[tenure]
    )


💡 Business Recommendations

    Encourage migration to long-term contracts

    Improve onboarding experience in the first 3–6 months

    Enhance fiber service quality and pricing transparency

    Promote automatic payment methods

    Implement targeted retention campaigns for high-risk segments

🛠 Tools & Technologies

    Power BI Desktop

    DAX (Data Analysis Expressions)

    Power Query

    Microsoft Excel / CSV dataset

🚀 How to Use This Project

    Clone the repository

    Open the .pbix file in Power BI Desktop

    Explore interactive dashboards

    Use slicers to analyze specific customer segments

📌 Conclusion

    This project demonstrates how data analytics and visualization can support strategic business decisions by:

    Identifying churn drivers

    Understanding customer behavior

    Improving retention strategies

    Enhancing customer lifetime value

SNAPSHOTS:
 DASHBOARD:
   PAGE1-
       ![Alt text](https://github.com/utkarsh695/FUTURE_DS_02/blob/main/snapshot1.png)
       [Dashboard](https://github.com/utkarsh695/FUTURE_DS_02/blob/main/snapshot1.png)

   NEXT-
       ![Alt text](https://github.com/utkarsh695/FUTURE_DS_02/blob/main/snapshot2.png)
      [Dashboard](https://github.com/utkarsh695/FUTURE_DS_02/blob/main/snapshot2.png)


   
