# Velour Coffee Shop Sales Analysis

Tools Used: Excel with Power Query <br>
Project Type: Data Cleaning, Exploratory Data Analysis (EDA), Dashboard Development

## Project Background
Founded in 2018, Velour Coffee Shop is a boutique-style café known for its artisanal coffee blends, inviting ambiance, and strong neighborhood presence across multiple New York locations. As the business continues to grow, Velour aims to leverage data to better understand customer behavior, sales trends, and product performance. <br>

The company has gathered comprehensive data on transactions, product categories, store-level performance, customer footfall, and ordering patterns. This project involved partnering with the business team to clean, analyze, and visualize this data in an accessible dashboard using Excel and Power Query. <br>

Insights and recommendations are provided on the following key areas:
- Sales Trends by Day and Month: Evaluation of order volumes across different weekdays and months to identify patterns and optimize operations accordingly.
- Store-Level Performance: Comparative assessment of footfall and sales across Velour locations to guide operational decisions and promotional focus.
- Top Product Insights: Identification of best-selling items to inform product stocking and marketing strategy.
- Order Size Preferences: Analysis of size distribution (Small, Regular, Large) to align offerings with customer preferences and maximize revenue.
- Weekday Sales Distribution: Understanding daily footfall variations to refine weekday promotions and customer engagement strategies.


## Relevant Resources
- The raw dataset used for analysis can be accessed [here](https://github.com/DanielaRubianoB/Velour-Coffee-Sales-dashboard/blob/main/Raw_CoffeeShop.xlsx). <br>
- The final cleaned dataset and Excel dashboard can be downloaded [here](https://github.com/DanielaRubianoB/Velour-Coffee-Sales-dashboard/blob/main/CoffeeShop_Dashboard.xlsx). <br>
- A presentation slide deck prepared for stakeholders can be viewed here. <br>

## Data structure and initial checks
The Velour Coffee Shop dataset, as seen below, consists of one structured table: Transactions, with a total of over 150,000 records.  <br>

<p align="center">
  <img src="https://github.com/DanielaRubianoB/Velour-Coffee-Sales-dashboard/blob/main/images/ERD.png" alt="Preview" />
</p>


Prior to beginning the analysis, a variety of checks were conducted for quality control and to gain familiarity with the data structure. These checks included schema validation, relationship consistency, data type integrity and data cleaning.  <br>

To align the analysis with business needs, a set of stakeholder-oriented questions was outlined. These informed the creation of calculated fields, aggregations, and filters used in the dashboard. All data preparation steps were conducted in Excel using Power Query to streamline the cleaning and transformation processes.

## Executive summary
From January to June 2023, Velour Coffee Shop generated $698,812 in total revenue across three New York locations, with monthly sales peaking in May at $123,457. Friday accounted for the highest daily order volume at 21,701 transactions. Hell’s Kitchen led store-level performance, generating $236,511 in revenue, while Lower Manhattan posted the highest average transaction value (ATV) at $4.81. At the product level, Barista Espresso contributed $91,406 (24%) of total top-product revenue. Size analysis showed a strong preference for Regular and Large drinks. Key opportunities for growth and optimization will be addressed in the following sections. <br> 

Below is the overview page of the dashboard, and the full interactive version can be downloaded [here](https://github.com/DanielaRubianoB/Velour-Coffee-Sales-dashboard/blob/main/CoffeeShop_Dashboard.xlsx).

![Dashboard Preview](https://github.com/DanielaRubianoB/Velour-Coffee-Sales-dashboard/blob/main/images/dashboard.png)

## Insights Deep-Dive 
### Sales Trends by Day and Month
Time-based analysis reveals significant variation in monthly and weekday sales performance.
- May generated $123,457, representing a 28% increase compared to January—the lowest-performing month—indicating a potential seasonal uplift or stronger promotional activity.
- Friday's order volume was 6% higher than the weekday average and also 6% above Monday and Thursday, reinforcing its position as the strongest day for transactional activity.
- Saturday's sales were 5.5% below the weekly average, suggesting an opportunity to recapture lost weekend revenue through targeted campaigns.
- Weekday volumes remained stable, with Monday–Thursday fluctuating within a 2.1% range, supporting consistent weekday operational strategy.

<p align="center">
  <img src="https://github.com/DanielaRubianoB/bean-bloom-sales-dashboard/blob/main/images/SalesTrends.png" alt="Preview" />
</p>

### Store-Level Performance
Location-based analysis reveals differences in revenue efficiency relative to footfall.
- Hell’s Kitchen achieved $236,511.17 in revenue, which is 1.8% higher than Astoria despite only a 0.2% higher footfall, reflecting stronger average transaction value (ATV).
- Lower Manhattan’s ATV was $4.81, 9.6% higher than Astoria’s and 6.3% higher than Hell’s Kitchen, despite its lower footfall—highlighting effective monetization per visitor.
- These insights suggest potential for applying Hell’s Kitchen's product mix or pricing strategy to underperforming locations.


<p align="center">
  <img src="https://github.com/DanielaRubianoB/bean-bloom-sales-dashboard/blob/main/images/Customers.png" alt="Preview" />
</p>

### Top Product Insights
Product-level revenue contributions identify key sales drivers and growth areas.
- Barista Espresso led with $91,406.20, contributing 24% of total product-level sales, outperforming the next best product by 18.6%.
- Brewed Chai Tea and Hot Chocolate followed, with combined revenue of $149,498, together contributing 39% of total sales among top 5 items.
- Despite fewer units sold, Brewed Black Tea's revenue per unit was 15% higher than Brewed Chai Tea, highlighting pricing leverage and potential for focused promotion.

### Order Size Preferences
Sizing behavior analysis highlights preferences and areas for pricing optimization.
- Regular and Large sizes each accounted for 30% of total orders, while Small sizes contributed only 9%, confirming a dominant preference for medium-to-large beverages.
- Large size orders generated 12% more revenue per transaction than Regular, indicating opportunity for upselling through value messaging.
- 31% of orders were labeled 'Not Defined', creating a visibility gap in product mix analysis—addressing this could improve forecast accuracy and demand planning.

<p align="center">
  <img src="https://github.com/DanielaRubianoB/bean-bloom-sales-dashboard/blob/main/images/Country.png" alt="Preview" />
</p>

## Recommendations & Opportunities
- Weekend Sales Optimization: With Saturday revenue trailing by 7.5%, introducing weekend-focused promotions, community events, or seasonal campaigns could help shift traffic from weekdays to weekends and reduce revenue concentration risk.
- Location-Based Strategy Adjustment: Lower Manhattan’s ATV is 9.6% higher than Astoria’s, despite lower footfall. This suggests potential to replicate premium pricing strategies or product emphasis across lower-performing stores to drive per-customer revenue.
- Product Portfolio Enhancement: With Barista Espresso generating 24% of top-product revenue, reinforcing its visibility via bundles, loyalty perks, or limited-time variants could increase attachment rates. Underperforming but high-value items like Brewed Black Tea offer upsell potential through targeted recommendations.
- Size-Based Pricing and Promotion: As Regular and Large sizes make up 60% of orders, value-driven upselling from Regular to Large can improve revenue without increasing footfall.
- Data Integrity and Standardization: The high percentage of “Not Defined” values in the Size field presents a data quality concern. Improving POS system configuration or data entry standards will strengthen reporting accuracy and enable more granular customer insights.

## Key Questions for Stakeholders Prior to Project Advancement
These are some questions I asked stakeholders/project leads early on to better understand business goals, clarify assumptions, and ensure data interpretation aligned with operational context:
- Approximately 30% of the order records have undefined values in the Size field. Should these entries be retained in the analysis as-is, cleaned, or excluded? 
- Are there existing customer segments (e.g., loyalty members, first-time buyers) that should be incorporated into the analysis, or will the focus remain on aggregate behavior?
- Are there any recent changes in store operations, promotions, or product offerings that could impact sales patterns and should be considered when interpreting the data?
- Is this dashboard meant for one-time strategic use, or will it support ongoing performance tracking and reporting?


## Assumptions and Caveats
The following assumptions and limitations were made during the course of this project due to gaps in context, incomplete metadata, or missing documentation:
- As confirmed by stakeholders, 'Not Defined' values have been retained in the analysis to reflect the full scope of recorded sales and avoid data exclusion bias.
- Unit prices are assumed to be static over the analysis period. Any potential price changes, promotions, or discounts are not accounted for.
- The analysis is performed at the transaction level. Without customer identifiers, behavioral insights such as repeat visits, retention, or individual lifetime value are outside the scope.
- The dataset does not include cost data, so profitability and margin analysis were not part of this scope.

