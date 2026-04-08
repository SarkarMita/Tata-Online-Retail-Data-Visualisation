# 🛒 Tata Online Retail Sales & Demand Analytics Dashboard
> Data Visualisation: Empowering Business with Effective Insights
> Tata Group Virtual Experience Program | Forage | April 2026

---

## 📋 Table of Contents
- [About the Project](#about-the-project)
- [Background](#background)
- [Data Cleaning](#data-cleaning)
- [Question 1](#question-1--monthly-revenue-trend-ceo)
- [Question 2](#question-2--top-10-countries-by-revenue--quantity-cmo)
- [Question 3](#question-3--top-10-customers-by-revenue-cmo)
- [Question 4](#question-4--global-product-demand-map-ceo)
- [Key Business Insights](#key-business-insights)
- [Tools Used](#tools-used)
- [Certificate](#certificate)
- [Connect With Me](#connect-with-me)

---

## 📌 About the Project

This project was completed as part of the **Tata Group Data 
Visualisation: Empowering Business with Effective Insights** 
virtual experience program on **Forage**.

The CEO and CMO of an online retail store requested data 
analysis and visualisations to help them make meaningful, 
data-driven decisions. The goal was to provide insights 
that would help the executives create an **expansion 
strategy** and understand the main factors affecting 
the online store's revenue generation.

---

## 🏢 Background

The CEO and CMO recently met to finalise their requirements 
and needed analysis across four key business questions. 
Both executives wanted clear, actionable insights that 
could be used to drive strategic business decisions and 
identify the most lucrative expansion opportunities 
for the business.

---

## 🧹 Data Cleaning

Before building any visuals, the raw data was carefully 
cleaned by applying the following quality checks:

**Check 1 — Quantity Validation**
- Condition: Quantity should not be below 1 unit
- Reason: Negative quantities represent product returns 
  which would distort revenue calculations
- Action: All records with Quantity less than 1 were 
  excluded from the analysis

**Check 2 — Unit Price Validation**
- Condition: Unit Price should not be below $0
- Reason: Negative or zero unit prices were data entry 
  errors that would negatively impact revenue figures
- Action: All records with Unit Price less than $0 were 
  excluded from the analysis

These checks were applied using conditional formulas 
and data transformation methods in Power BI before 
any analysis was performed. This ensured all four 
visuals were built on accurate, clean and reliable data.

---

## 📊 Question 1 — Monthly Revenue Trend (CEO)

### Business Requirement
The CEO of the retail store is interested to view the 
time series of the revenue data for the year 2011 only. 
He would like to view granular data by looking into 
revenue for each month. The CEO is interested in viewing 
the seasonal trends and wants to dig deeper into why 
these trends occur. This analysis will be helpful for 
the CEO to forecast for the next year.

### Approach
- Filtered data to 2011 only
- Created a line chart with months on X-axis and 
  revenue on Y-axis
- Set X-axis type to Categorical to display all 
  12 months clearly
- Added data labels to each monthly data point

### Visual
![Q1 Monthly Revenue](https://github.com/SarkarMita/Tata-Online-Retail-Data-Visualisation/blob/main/Bar%20Chart.png)

### Findings

| Month | Revenue | Trend |
|---|---|---|
| January | 0.61M | Moderate start |
| February | 0.52M | Dip |
| March | 0.71M | Recovery |
| April | 0.51M | Lowest point |
| May | 0.76M | Growth |
| June | 0.75M | Stable |
| July | 0.71M | Slight dip |
| August | 0.72M | Stable |
| September | 1.04M | Strong growth |
| October | 1.11M | Continued growth |
| November | 1.49M | Peak revenue |
| December | 0.47M | Sharp decline |

### Key Insights
- Revenue shows a clear seasonal pattern with 
  strong Q4 performance
- November is the peak month at 1.49M driven by 
  holiday season shopping
- April is the lowest month at 0.51M
- Consistent upward trend from August to November
- December decline is likely due to incomplete 
  data for that month

### Business Recommendation
The CEO should plan higher inventory levels and 
increased marketing spend for September through 
November to capitalise on peak seasonal demand 
and maximise revenue for the following year.

---

## 📊 Question 2 — Top 10 Countries by Revenue & Quantity (CMO)

### Business Requirement
The CMO is interested in viewing the top 10 countries 
which are generating the highest revenue. Additionally, 
the CMO is also interested in viewing the quantity sold 
along with the revenue generated. The CMO does not want 
to have the United Kingdom in this visual.

### Approach
- Applied Top N filter to show top 10 countries by revenue
- Excluded United Kingdom using basic filter
- Used Clustered Column Chart to show both Revenue 
  and Quantity side by side
- Sorted by descending revenue order

### Visual
![Q2 Top 10 Countries](screenshots/Q2_Top10_Countries.png)

### Findings

| Rank | Country | Revenue | Quantity Sold |
|---|---|---|---|
| 1 | Netherlands | 285K | 200K |
| 2 | EIRE | 275K | 143K |
| 3 | Germany | 226K | 118K |
| 4 | France | 199K | 111K |
| 5 | Australia | 138K | 83K |
| 6 | Spain | 58K | 27K |
| 7 | Switzerland | 57K | 30K |
| 8 | Belgium | 41K | 23K |
| 9 | Sweden | 37K | 36K |
| 10 | Norway | 36K | 19K |

### Key Insights
- Netherlands leads with 285K revenue and 200K units sold
- Europe dominates all top 10 positions except Australia
- Australia is the only non-European country in the top 5
- Sweden has relatively lower revenue but high quantity 
  sold suggesting lower priced products are popular there

### Business Recommendation
The CMO should focus customer retention strategies on 
Netherlands, EIRE and Germany as they are the highest 
value markets. Australia represents a strong growth 
opportunity outside Europe.

---

## 📊 Question 3 — Top 10 Customers by Revenue (CMO)

### Business Requirement
The CMO of the online retail store wants to view the 
information on the top 10 customers by revenue. He is 
interested in a visual that shows the greatest revenue 
generating customer at the start and gradually declines 
to the lower revenue generating customers. The CMO wants 
to target the higher revenue generating customers and 
ensure that they remain satisfied with their products.

### Approach
- Applied Top N filter to show top 10 customers by revenue
- Used Horizontal Bar Chart for clear readability 
  of Customer IDs
- Sorted highest to lowest revenue as requested by CMO
- Changed CustomerID data type to Text for proper 
  display on axis

### Visual
![Q3 Top 10 Customers](screenshots/Q3_Top10_Customers.png)

### Findings

| Rank | Customer ID | Revenue |
|---|---|---|
| 1 | 14646 | 280K |
| 2 | 18102 | 260K |
| 3 | 17450 | 190K |
| 4 | 14911 | 139K |
| 5 | 12415 | 124K |
| 6 | 14156 | 115K |
| 7 | 17511 | 88K |
| 8 | 16029 | 66K |
| 9 | 16684 | 66K |
| 10 | 14096 | 65K |

### Key Insights
- Customer 14646 is the highest value customer 
  generating 280K in revenue
- Top 2 customers together generate 540K which is 
  a significant portion of total revenue
- There is a notable gap between rank 2 (260K) 
  and rank 3 (190K)
- The bottom 3 customers each generate similar 
  revenue around 65-66K
- Revenue gradually declines from top to bottom 
  as required by CMO

### Business Recommendation
The CMO should immediately implement a VIP customer 
retention program targeting customers 14646 and 18102. 
Losing either of these customers would have a significant 
negative impact on overall revenue. Personalised offers, 
dedicated account managers and exclusive benefits should 
be considered for these top customers.

---

## 📊 Question 4 — Global Product Demand Map (CEO)

### Business Requirement
The CEO is looking to gain insights on the demand for 
their products. He wants to look at all countries and 
see which regions have the greatest demand for their 
products. Once the CEO gets an idea of the regions that 
have high demand, he will initiate an expansion strategy 
which will allow the company to target these areas and 
generate more business from these regions. He wants to 
view the entire data on a single view without the need 
to scroll or hover over the data points to identify the 
demand. There is no need to show data for the United 
Kingdom as the CEO is more interested in viewing the 
countries that have expansion opportunities.

### Approach
- Used Bubble Map visual in Power BI
- Set Country as location field
- Set Sum of Quantity as bubble size so larger bubble 
  means higher demand
- Excluded United Kingdom using filter
- Enabled Category labels to show country names on map
- Resized map to fill entire canvas for single view 
  with no scrolling

### Visual
![Q4 Global Demand Map](screenshots/Q4_Global_Demand_Map.png)

### Findings

| Region | Demand Level | Expansion Opportunity |
|---|---|---|
| Europe (France, Netherlands, Germany) | Very High | Low — already established |
| Australia | Moderate | Medium — room to grow |
| Japan | Low to Moderate | Medium — untapped potential |
| North America | None | Very High |
| South America | None | Very High |
| Africa | None | Very High |
| Middle East | Very Low | High |
| Southeast Asia | Very Low | High |

### Key Insights
- Europe has the highest concentration of product 
  demand globally
- Australia and Japan show moderate demand signals 
  outside Europe
- North America, South America and Africa show 
  virtually no demand representing the biggest 
  expansion opportunities
- The entire world map is visible in one single 
  view with no scrolling required

### Business Recommendation
The CEO should prioritise Asia Pacific as the first 
expansion region given existing demand signals from 
Australia and Japan. North America would be the second 
priority given its large market size. Africa and South 
America represent longer term expansion opportunities.

---

## 💡 Key Business Insights

| Question | Key Finding | Recommendation |
|---|---|---|
| Q1 Seasonal Trends | Peak in November at 1.49M | Plan inventory and marketing for Q4 |
| Q2 Top Markets | Netherlands, EIRE, Germany lead | Focus retention in top European markets |
| Q3 Top Customers | Customer 14646 and 18102 dominate | Launch VIP customer retention program |
| Q4 Global Demand | North America and Asia untapped | Prioritize Asia Pacific for expansion |

---

## 🛠️ Tools Used

- **Power BI Desktop** — Dashboard and visualisation creation
- **Microsoft Bing Maps** — Global demand bubble map
- **Microsoft Excel** — Raw data source
- **Forage Platform** — Virtual experience program

---

## 🏆 Certificate

Successfully completed the **Tata Group Data Visualisation: 
Empowering Business with Effective Insights** virtual 
experience program on Forage.

- 📅 Completed: April 8th, 2026
- 🎓 Issued by: Forage
- 🏢 Program by: Tata Group

![Completion Certificate](certificate/completion_certificate.png)

---

## 🔗 Connect With Me

I am always open to discussing data analytics, 
visualisation projects and collaboration opportunities.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mita%20Sarkar-blue?style=for-the-badge&logo=linkedin)](www.linkedin.com/in/mita-sarkar-mba-analyst)
[![GitHub](https://img.shields.io/badge/GitHub-SarkarMita-black?style=for-the-badge&logo=github)](https://github.com/SarkarMita)
[![Email](https://img.shields.io/badge/Email-Contact%20Me-red?style=for-the-badge&logo=gmail)](mitasarkar7727@gmail.com)

---

⭐ If you found this project helpful please 
consider giving it a star!
