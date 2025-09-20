## TITLE
TELECOM CUSTOMER CHURN ANALYSIS

## SUMMARY
A comprehensive data analysis project analyzing telecom customer churn patterns, conducted as part of the STC 6-Week Data Analyst Mentorship. The project includes data cleaning, analysis, visualization, and actionable recommendations to reduce customer churn and improve retention strategies.

## INTRODUCTION
This project analyzes telecom customer data to understand churn patterns and identify factors contributing to customer attrition. With the telecommunications industry facing increasing competition and customer acquisition costs, understanding why customers leave and developing effective retention strategies is crucial for business sustainability and growth.

## PROJECT DESCRIPTION
The project covers a complete end-to-end data analysis workflow including data exploration, cleaning, analysis, visualization, and strategic recommendations. The analysis spans 4 weeks of intensive work, from initial business question framing to final dashboard creation and stakeholder recommendations.

## PROJECT AIM
To analyze telecom customer data to identify churn patterns, understand customer behavior, and provide actionable recommendations for stakeholders to reduce customer churn and improve retention rates.

## ABOUT THE DATASET
* **Source**: Telecom Company Customer Database
* **Number of Records**: 7,043 customers
* **Key Metrics**: $21.37M total revenue, $3.68M revenue lost to churn
* **Key Fields**: 
  *	Customer Demographics (Age, Gender, Marital Status)
  *	Service Information (Phone Service, Internet Service, Multiple Lines)
  *	Contract Details (Contract Type, Payment Method, Tenure)
  *	Service Add-ons (Device Protection, Online Security, Streaming Services)
  *	Churn Status and Financial Impact
    
## TOOLS USED
* Microsoft Power BI - Dashboard creation and data visualization
*	Microsoft Excel - Initial data exploration and validation
*	Figma – For designing dashboard background
  
## IMPORTING THE DATASET
The telecom customer dataset was imported directly into Power BI for comprehensive analysis and visualization. Data validation and initial exploration were conducted to understand the structure and quality of the dataset before proceeding with analysis.

## DATA CLEANING & TRANSFORMATION
**Data Quality Assessment:**
The dataset was relatively clean but required specific attention to handle missing values appropriately.

**Issues Identified:**
* Empty cells in dependent columns: Some columns had blank values due to logical dependencies on other columns. For instance, if Internet Service = "No" (customer did not subscribe to internet), then Internet Type was blank for that row.
* Null values in numeric columns: Fields like Avg Monthly Long Distance Charges contained null values because customers had not subscribed to home phone service.

**Cleaning Steps Performed:**
* Replaced null values in numeric columns with 0 - This accurately represented customers who didn't use specific services
* Replaced null text values with "Unknown" - Applied only to columns not dependent on other service subscriptions
* Maintained logical data relationships - Preserved the dependency structure between service subscription and related fields

**Data Structure:**
* No changes were made to column names as they were already in readable and clear format
* Preserved original data dictionary alignment for consistency and accuracy

## DATA ANALYSIS
Some key metrics analyzed
*	Customer Churn Rate (26.54%)
*	Revenue Impact ($3.68M lost)
*	Service Adoption Rates (Phone: 90.32%, Internet: 78.33%, Multiple Lines: 42.18%)
*	Customer Demographics (Average Age: 47, Average Tenure: 32 months)
*	Contract Distribution and Payment Preferences
*	Geographic Customer Distribution
*	Service Add-on Utilization Rates
  
## DATA VISUALIZATION
**Service Overview Dashboard**

**KPI Cards - Financial Performance**
* Total Revenue of $21.37M demonstrates strong market presence and customer base value
* Average Monthly Charges of $63.60 indicates competitive pricing in the telecom market
* Phone Service leads adoption at 90.32%, showing near-universal customer engagement
* Internet Service adoption at 78.33% indicates strong digital service demand
* Multiple Line adoption at 42.18% suggests opportunities for family/business package growth

**Customer Distribution by Promotional Offers**

**Chart**: Vertical bar chart showing customer counts across different promotional offers.

**Key Insights**:
* Majority of customers (3,877) have not taken any promotional offers, indicating potential for targeted marketing campaigns
* Offer B shows the highest uptake among promotional offers, closely followed by offer B suggesting this package resonates well with customers
* Low uptake on other offers (A, C, D) suggests need for offer restructuring or better marketing

**Contract Types Distribution**

**Chart**: Vertical bar chart showing customer counts across different promotional offers

**Key Insights:**
* Month-to-month contracts dominate at 51.26%, indicating customer preference for flexibility but also higher churn risk
* Two-year contracts represent 26.72% of customers, showing some commitment to longer terms
* One-year contracts at 22.01% represent the smallest segment, suggesting this option may need repositioning

**Payment Methods Distribution**

**Chart**: Donut chart showing customer payment method preferences

**Key Insights:**
* Bank Withdrawal is preferred by 55.5% of customers, indicating trust in automated payments and good cash flow predictability
* Credit Card payments at 39.03% show digital payment adoption
* Mailed Check at 5.47% represents traditional payment preferences, potentially from older demographics

**Internet Service Types**

**Chart**: Horizontal bar showing customer counts by internet service type

**Key Insights:**
* Fiber Optic leads significantly with 3,035 customers, demonstrating strong infrastructure investment returns
* DSL follows with 1,652 customers, showing continued demand for traditional broadband
* Cable with 830 customers represents the smallest segment, possibly due to infrastructure limitations

**Service Add-on Adoption**

**Chart**: Stacked bars showing Yes/No distribution for each service add-on

**Key Insights:**
* Device Protection Plan leads adoption at 65.19%, indicating customer value perception for device security
* Online Backup (63.85%) and Online Security (63.40%) show strong digital safety awareness
* Streaming services show balanced adoption: TV (50.83%) and Music (54.08%) indicating entertainment service demand
* Premium Tech Support has lowest adoption at 37.50%, suggesting either price sensitivity or satisfaction with standard support

**Customer Demographics Dashboard**

**KPI Cards - Customer Overview**
* Customer base of 7,043 represents substantial market presence
* Average age of 47 indicates mature customer demographic with established purchasing power
* Average tenure of 32 months shows reasonable customer loyalty and lifecycle length

**Age Groups and Gender Distribution**

**Chart**: Stacked bars showing customer and churn distribution across age groups by gender

**Key Insights**:
* 18-29 years: 681 customers with 501 churned (21.30% churn rate) - lowest churn demographic
* 30-39 years: 1,649 customers with 891 churned (24.34% churn rate)
* 40-49 years: 1,449 customers with 841 churned (24.52% churn rate)
* 50-64 years: 1,588 customers with 897 churned (30.38% churn rate)
* 65+ years: 1,676 customers with 1,737 churned (41.68% churn rate) - highest risk group
* Gender distribution appears relatively balanced across all age segments

**Marital Status Distribution**

**Chart**: Donut chart displaying marital status breakdown

**Key Insights:**
* Single customers represent 48.1% (3,386) of the customer base, indicating strong individual customer market
* Married customers at 43.7% (3,078) show significant family market presence
* Remaining 8.2% (579) represents other marital statuses
* Distribution suggests need for both individual and family-oriented service packages

**Tenure Groups Distribution**

**Chart**: Donut chart showing customer distribution by tenure ranges

**Key Insights:**
* Short-term: 22.85% with 47.44% churn rate - critical early retention period
* Mid-term: 31.78% with 30.48% churn rate - stabilizing period
* Long-term: 45.37% with 6.76% churn rate - loyal customer base
* Distribution shows successful long-term retention but early-stage challenges
  
**Customers By Dependents Analysis**

**Charts**: Line and column charts showing customer distribution by number of dependents.

**Key Insights:**
* 0 Dependents: Highest customer count with 30.06% churn rate
* 1-3 Dependents: Progressive decrease in churn rates (18.89%, 13.89%, 10.00%)
* 4+ Dependents: Lowest churn at 8.33% - family stability drives retention

**Customers By Referrals Analysis**

**Charts**: Line and column charts showing customer distribution by number of and referrals

**Key Insights:**
* 0 Referrals: 33.05% churn rate - highest risk customers
* 1-3 Referrals: Decreasing churn rates (15.79%, 11.67%, 8.70%)
* 4+ Referrals: Lowest churn at 6.25% - engaged customers stay longer.
  
**Churn Analysis & Financial Impact Dashboard**

**KPI Cards - Churn Metrics**
* $3.68M revenue lost represents 17.2% of total revenue, indicating significant financial impact
* 26.54% churn rate is concerning and above industry benchmarks, requiring immediate attention
* 67.02% retention rate shows majority customer satisfaction but room for improvement
* Churned customers average only 18 months tenure vs 32 months overall, highlighting early-stage retention challenges

**Membership Status Distribution**

**Chart**: Pie chart showing breakdown of customer membership status (67.02% Stayed, 26.54% Churned)

**Key Insights:**
* Visual representation confirms that over 1 in 4 customers are churning
* 67.02% retention rate provides foundation for improvement strategies
* Clear visualization of the revenue protection opportunity through churn reduction.

**Churn Rate by Age Group**

**Chart**: Vertical bar chart displaying churn rates across age segments

**Key Insights:**
* 18-29 years: 21.30% churn rate - most loyal demographic requiring retention rewards
* 30-39 years: 24.34% churn rate - career-building phase with competitive sensitivity
* 40-49 years: 24.52% churn rate - stable demographic with moderate risk
* 50-64 years: 30.38% churn rate - pre-retirement concerns driving switches
* 65+ years: 41.68% churn rate - highest risk requiring specialized senior programs
  
**Churn Rate by Tenure Range**

**Chart:** Vertical bar chart showing churn rates across tenure periods

**Key Insights:**
* Short-term: 47.44% churn rate - critical onboarding and early experience issues
* Mid-term: 30.48% churn rate - relationship building period challenges
* Long-term: 6.76% churn rate - demonstrates loyalty program success potential

**Churn Rate by Contract Type**

**Chart**: Vertical bar chart displaying churn rates for different contract types

**Key Insights:**
* Month-to-Month: 42.71% churn rate - high flexibility correlates with high attrition
* One-Year: 10.79% churn rate - moderate commitment shows retention improvement
* Two-Year: 2.83% churn rate - long-term contracts dramatically reduce churn risk

**Service Category and Offer Analysis**

**Charts**: Multiple horizontal bar charts showing churn rates by service categories and promotional offers

**Key Insights:**
* Churn by Category: Competitor (41.68%), Dissatisfaction (39.12%), Attitude (38.83%), Price (31.26%), Other (9.74%)
* Churn by Offer: No Offer customers show highest churn risk, while Offer E shows best retention
* Service-specific analysis reveals Device Protection and Online Security as retention drivers
* Premium services show mixed retention impact requiring optimization
  
## KEY INSIGHTS
* **Critical Churn Rate**: 26.54% churn rate resulting in $3.68M annual revenue loss
* **Contract Impact**: Month-to-month customers show significantly higher churn compared to long-term contracts
* **Tenure Correlation**: Churned customers average only 18 months tenure vs. 32 months overall average
* **Service Satisfaction**: High service adoption rates (90%+ phone, 78%+ internet) indicate strong service quality
* **Payment Preference**: 59.25% customers prefer automated bank withdrawal payments
* **Service Leader**: Fiber Optic dominates internet services with 3,096 customers
* **Add-on Success**: Device Protection Plan leads service add-ons with 65.19% adoption
* **Geographic Diversity**: Customer base spans multiple continents with strong international presence
  
## RECOMMENDATIONS
**For senior management & executives**
* Implement comprehensive customer retention strategy with quarterly churn reduction targets
* Prioritize infrastructure investment in Fiber Optic expansion
* Develop strategic partnerships with streaming platforms for bundled offerings.
  
**For customer retention team**
* Create intensive 18-month customer success program with regular check-ins and milestone rewards.
  
**For marketing department**
* Design attractive incentive packages (15-20% discounts) for annual/bi-annual contract conversions
* Develop age-specific and region-specific marketing campaigns
* Leverage Device Protection Plan success to cross-sell other services.
  
**For service development team**
* Invest in advanced digital services development based on high online service adoption rates.
  
**For customers support managers**
* Offer additional incentives for automated payment method adoption to improve cash flow predictability.
  
## CONCLUSION
The analysis reveals that while the telecom company maintains strong service adoption rates and customer satisfaction, the 26.54% churn rate represents a significant revenue risk. The clear correlation between contract length and retention, combined with high service satisfaction scores, suggests that strategic retention initiatives focusing on contract optimization and early customer success programs could substantially reduce the $3.68M annual revenue loss. Coordinated action across all departments, emphasizing customer lifecycle extension and value proposition enhancement, will be critical for building a more sustainable and profitable customer base

## CONTACT INFORMATION

* LinkedIn: https://www.linkedin.com/in/mariamolatunji
* Email: oyinkansolamariam17@gmail.com
* GitHub: https://github.com/olamariam17

