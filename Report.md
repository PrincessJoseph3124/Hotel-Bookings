# Hotel Bookings Analysis: Revenue Optimization & Customer Behavior Intelligence

**Business Problem / Objective**

Hotel management wants to understand booking performance, revenue drivers, and customer behavior patterns to optimize pricing, reduce cancellations, and improve guest retention.

The business needs clear visibility into:

- How booking volume and revenue trend over time

- What drives cancellations and how to reduce them

- Which market segments and customer types generate the most revenue

- How booking lead time affects revenue and cancellations

- Which countries and regions contribute most to performance

- How repeat guests impact profitability

This project answers the core question:

**How can the hotel optimize revenue performance while improving booking stability and guest retention?**

**Dataset Overview**

- Data Source: Hotel booking dataset 

- Time Period Covered: Multi-year booking records

- Volume: 100,000+ booking records

- Geography: Global customer distribution

**Key Columns in the Dataset**

- Booking ID

- Arrival Date (Year, Month, Day)

- Lead Time (Days before arrival)

- Hotel Type (City / Resort)

- Market Segment

- Distribution Channel

- Customer Type (Transient, Contract, Group, etc.)

- Reserved Room Type

- Assigned Room Type

- ADR (Average Daily Rate)

- Total Nights Stayed

- Total Revenue

- Cancellation Status

- Country

- Repeat Guest Flag

**Tools Used**

Looker Studio – Data visualization & dashboard development

Excel / Power Query – Data cleaning and preparation

SQL – Data exploration and aggregation

**Data Cleaning & Preparation**

- Removed duplicate booking records

- Handled missing values in ADR, country, and customer fields

- Standardized date formats for time intelligence

 Created calculated fields:

- Total Revenue = ADR × Total Nights

- Booking Month

- Booking Year

- Cancellation Rate

- Repeat Guest %

- Converted categorical fields into consistent labels

- Created clean dimensions (Date, Customer Type, Market Segment, Geography)

**Data Modeling**

- Separated fact table (Bookings) from dimension attributes

- Created calculated measures:

- Total Bookings = COUNT(Booking ID)

- Total Revenue = SUM(Total Revenue)

- Cancellation Rate = Canceled Bookings ÷ Total Bookings

- Average Lead Time = AVG(Lead Time)

- Repeat Guest % = Repeat Guests ÷ Total Guests

- Revenue by Segment

- Revenue by Customer Type

**Key Questions & Analysis**

- What is the overall booking volume and revenue performance?

- What percentage of bookings are canceled?

- Which market segments generate the highest revenue?

- How does lead time impact cancellation likelihood?

- Which countries are top revenue contributors?

- What is the split between repeat and new guests?

- Which room types generate the most revenue?

**Key Insights**

- Total Bookings: 119K+

- Total Revenue: $43M+

- Cancellation Rate: 37% (indicating high revenue leakage risk)

- Average Lead Time: 104 days

- Repeat Guest Rate: 3.19% (low retention opportunity)

- Transient customers generated the majority of revenue (~80%)

- Online Travel Agencies contributed heavily to bookings

- Certain room types drive disproportionately high revenue

- Revenue trends show seasonal peaks and off-peak slowdowns

**Recommendations**

- Implement flexible cancellation policies for long lead-time bookings

- Develop loyalty incentives to increase repeat guest rate beyond 5%

- Focus marketing on high-performing market segments

- Optimize pricing strategies during peak seasons

- Reduce dependency on high-commission distribution channels

- Promote direct booking incentives to improve profit margins

**Dashboard / Visualization**

The Tableau project contains two main dashboards:

**1️. Customer Booking Behavior & Operational Trends**

- Total bookings KPI

- Cancellation rate KPI

- Average lead time KPI

- Repeat guest %

- Monthly revenue trend

- Booking behavior by customer type

- Lead time trend analysis

- Geographic booking distribution

**2️. Revenue & Market Segment Performance**

- Revenue by customer type

- Top-performing market segments

- Top revenue-generating countries

- Room type performance breakdown

- Cancellation rate comparison by room type

- Revenue contribution analysis

**Conclusion**

This Hotel Bookings Analysis transformed raw booking data into actionable insights that help management:

- Identify revenue drivers and leakage risks

- Understand customer behavior and booking patterns

- Detect seasonality and performance fluctuations

- Improve strategic pricing and retention decisions

The dashboards provide hotel stakeholders with a centralized performance intelligence tool to monitor revenue, reduce cancellations, and drive sustainable growth.

**Limitations**

Dataset does not include marketing spend data

No detailed guest demographic segmentation

External factors (economic conditions, events, seasonality drivers) not included

Historical dataset may not reflect current market dynamics
