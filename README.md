# FMCG-Supply-Chain-Analysis

[Live Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMWFiZGRiOTMtMjllNS00ZGFjLWI1NjItOTgzZjc3MDA0NDkxIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

[Video Presentation HD](https://www.youtube.com/embed/ccVVqyDH2vA?si=M90reYfy6Lwg5rrg)

[LinkedIn Post](https://www.linkedin.com/posts/mrajesh1312_codebasicsresumeprojectchallenge2-codebasicsresumeprojectchallenge2-activity-7135553059589398528-ZjQc?utm_source=share&utm_medium=member_desktop)

[This Project Resources](https://codebasics.io/challenge/codebasics-resume-project-challenge)

***
## Table of Content 

- [About Company](#About-Company)
- [Problem Statement](#Problem-Statement)
- [Management request](#Management-request)
- [Key service metrics](#Key-service-metrics)
- [My Role in this project](#My-Role-in-this-project)
- [Data sets](#Data-sets)
- [Dashboard](#Dashboard)
- [Insights](#Insights)

***
## About Company

- AtliQ Mart is a growing FMCG manufacturer headquartered in Gujarat, India. It is currently operational in three cities 

  **1.Surat**

  **2.Ahmedabad**

  **3.Vadodara**

  ***
## Problem Statement

- AtliQ Mart aims to expand its operations to other metro cities within the next two years.
- However, the company is currently facing a critical challenge. Several key customers have not renewed their annual contracts due to service issues.
- These problems are mainly related to the delivery of essential products. 
- On several occasions, these products were either not delivered **On Time** or not delivered **In Full** over an extended period.
- This has resulted in poor customer service and dissatisfaction.

***
## Management request

- Management has identified service issues and aims to address them before expanding to new cities. 
- They have instructed the supply chain analytics team to monitor daily **On-time** and **In Full** delivery service levels for all customers to enable prompt issue resolution.

***
## Key service metrics

- The Supply Chain team employs a standardized approach for measuring service levels.
- Key metrics include

  **Total Orders**
  
   **Total Orders Lines**

   **On-time delivery (OT)%**

   **In-full delivery(IF)%**

   **Line Fill Rate (LIFR)%**

   **Volume Fill Rate (VOFR)%**
- The team monitors **Total Order** and **Total Order Lines** for daily customer orders.
- These metrics are compared against the target service levels established for each customer.

***
## My Role in this project

- Hi, **I’m Rajesh**, the data analyst in the supply chain team at AtliQ Mart. 
- I recently joined the company and briefed about the task in the stakeholder business review meeting. 
- Today, I'm excited to discuss the role I'll be building a dashboard to address the supply chain challenges.

***
## Data sets

<details> 
<summary>
 Click here for Meta data(Details of Data Sets)

</summary>

***

This file contains all the meta information regarding the columns described in the CSV files. we have provided 3 CSV files:

- [dim customers](#dim-customers)

- [dim products](#dim-products)

- [dim date](#dim-date)

- [dim targets orders](#dim-targets-orders)

- [fact order lines](#fact-order-lines)

- [fact orders aggregate](#fact-orders-aggregate)

---------------------------------------------------------------------------------------------

## dim customers

This table contains all the information about customers

**1. customer_id:** Unique ID is given to each customer

**2. customer_name:** Name of the customer

**3. city:** It is the city where the customer is present

---------------------------------------------------------------------------------------------------

## dim products
This table contains all the information about the products

**1. product_name:** It is the name of the product

**2. product_id:** Unique ID is given to each of the products

**3. category:** It is the class to which the product belongs

---------------------------------------------------------------------------------------------------

## dim date
This table contains the dates at daily, monthly level and week numbers of the year

**1. date:** date at the daily level

**2. mmm_yy:** date at the monthly level

**3. week_no:** week number of the year as per the date column

---------------------------------------------------------------------------------------------------

## dim targets orders
This table contains all target data at the customer level

**1.customer_id:** Unique ID that is given to each of the customers

**2.ontime_target %:** Target assigned for Ontime % for a given customer

**3.infull_target %:** Target assigned for infull % for a given customer

**4.otif_target %:**   Target assigned for otif % for a given customer

---------------------------------------------------------------------------------------------------
## fact order lines
This table contains all information about orders and each item inside the orders.

**1. order_id:** Unique ID for each order the customer placed

**2. order_placement_date:** It is the date when the customer placed the order

**3. customer_id:** Unique ID that is given to each of the customers

**4. product_id:** Unique ID that is given to each of the products

**5. order_qty:** It is the number of products requested by the customer to be delivered

**6. agreed_delivery_date:** It is the date agreed between the customer and Atliq Mart to deliver the products

**7. actual_delivery_date:** It is the actual date Atliq Mart delivered the product to the customer

**8. delivered_qty:** It is the number of products that are actually delivered to the customer


---------------------------------------------------------------------------------------------------

## fact orders aggregate
This table contains information about OnTime, InFull and OnTime Infull information aggregated at the order level per customer

**1. order_id:** Unique ID for each order the customer placed

**2. customer_id:** Unique ID that is given to each of the customers

**3. order_placement_date:** It is the date when the customer placed the order

**4. on_time: '1'** denotes the order is delviered on time. '0' denotes the order is not delivered on time.

**5. in_full: '1'** denotes the order is delviered in full quantity. '0' denotes the order is not delivered in full quantity.

**6: otif:    '1'** denotes the order is delviered both on time and in full quantity. '0' denotes the order is either not delivered on time or not in full quantity.

</details> 

***

## Dashboard


[Live Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMWFiZGRiOTMtMjllNS00ZGFjLWI1NjItOTgzZjc3MDA0NDkxIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

*** 
## Insights

### Key Metrics By Cities

<img width="600" alt="image" 
  src="https://github.com/rajeshkumar1312/FMCG-Supply-Chain-Analysis/blob/main/Resources/Spite%20by%20city.png">

- Ahmedabad, Surat, and Vadodara are not meeting the targets for On-time Delivery (OT%) and On Time in Full (OTIF%), highlighting performance gaps in these areas.

- The primary focus should be on enhancing OT% and OTIF% to improve overall service quality and avoid customer dissatisfaction.

- Operational adjustments might be necessary to ensure orders are delivered on time and in full, aligning with the established targets.

***

### Product Insights

<img width="600" alt="image" 
  src="https://github.com/rajeshkumar1312/FMCG-Supply-Chain-Analysis/blob/main/Resources/Product%20insights.png">

- Some products may not be fully delivered (LIFR%: 66%), while most of the ordered volume is fulfilled (VOFR%: 97%).

- Understanding why certain products face delivery issues, such as order processing or stock availability, can improve overall delivery.

- To enhance efficiency, we'll optimize processes and improve communication with suppliers, using these insights keep refining our processes for ongoing enhancement.

***

### Customer Insights


<img width="600" alt="image" 
  src="https://github.com/rajeshkumar1312/FMCG-Supply-Chain-Analysis/blob/main/Resources/Customers%20insights.png">
  
- Key customers like Cool Blue, Acclaimed Stores, and Lotus Mart are experiencing delays in receiving their orders on time, indicating potential issues with delivery timelines.

- Elite Mart, Soreforz Mart, and Info Stores struggle with delivering complete orders, possibly leading to customer dissatisfaction due to incomplete deliveries.

- Expression Stores, Logic Stores, and Chiptec Stores exhibit better performance in providing complete orders, ensuring higher customer satisfaction.

- Propel Mart, Expert Mart, and Vivek Stores excel in meeting both delivery timelines and providing complete orders, demonstrating superior delivery service compared to others.

***

### Performance Over Time

#### On Time% (OT%) and Targets

<img width="600" alt="image" 
  src="https://github.com/rajeshkumar1312/FMCG-Supply-Chain-Analysis/blob/main/Resources/OT%25%20and%20Target.png">

#### In Full% (If%) and Target
<img width="600" alt="image" 
  src="https://github.com/rajeshkumar1312/FMCG-Supply-Chain-Analysis/blob/main/Resources/IF%25%20and%20Target.png">

#### On Time In Full% (OTIF%) and Target
<img width="600" alt="image" 
  src="https://github.com/rajeshkumar1312/FMCG-Supply-Chain-Analysis/blob/main/Resources/OTIF%25%20and%20Target.png">
  
- The key performance metrics, including On-time Delivery (OT%), In-full Delivery (IF%), and On Time in Full (OTIF%), have not reached their targets over time.

- This shortfall indicates a consistent trend where the actual performance of these metrics.

- Failure to meet these key performance indicators (KPIs) might signify challenges or inefficiencies in the delivery process that need to be addressed.

***

### Delay Deliveries

<img width="600" alt="image" 
  src="https://github.com/rajeshkumar1312/FMCG-Supply-Chain-Analysis/blob/main/Resources/Delay%20delivery-%20supply%20chain%20analysis.png">

- 37k orders are delivered on time, the largest segment.
- 3.6k orders arrive a day early, showing some early deliveries.
- 8.3k orders face a one-day delay, while 5.1k and 3.1k are delayed by two and three days.
- Most deliveries are on time or slightly late by a day, but a few face longer delays of two or three days.


***

### Total order lines with LIFR % of the customers 

<img width="600" alt="image" 
  src="https://github.com/rajeshkumar1312/FMCG-Supply-Chain-Analysis/blob/main/Resources/Order%20lines-%20Supply%20chain%20analysis.png">

- Vijay Stores, Rel Fresh, Lotus Mart, Propel Mart, and Acclaim Stores have the highest total order lines among customers.

- Higher total order lines may suggest greater demand or a wider range of products/services offered by these customers.

- Lower line fill rates for Cool blue, Elite Mart, and Info Stores could indicate potential challenges in meeting order requirements or fulfillment issues that need attention for improved customer service.

***



# THANK YOU😁
  
