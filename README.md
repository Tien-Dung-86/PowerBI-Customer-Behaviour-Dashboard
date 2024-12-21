# [Power BI] Customer Behaviour Analysis

## I. Introduction
<p>This project leverages the AdventureWorks database to conduct factors affecting the purchase of goods to serve the production of businesses,providing actionable insights for strategic purchases. Analysis classifies suppliers into separate segments based on their supply behaviors such as: Price, quality, delivery time. Tailored recommendations are provided to improve production availability, replace substandard suppliers, thereby optimizing marketing strategies and improving overall business performance. This Power BI project provides visual dashboards that enable data-driven decision making for effective supplier relationship management.</p>

### Dataset
Dataset: adventureworks2019 (public Google BigQuery dataset)

Dataset dictionary: https://github.com/Tien-Dung-86/PowerBI-Customer-Behaviour-Dashboard/blob/master/AdventureWorks%20_%20Data%20Dictionary.pdf

Data Schema: https://i0.wp.com/improveandrepeat.com/wp-content/uploads/2018/12/AdvWorksOLTPSchemaVisio.png?ssl=1

Dataset access:
- Log in to your Google Cloud Platform account and create a new project.
- Navigate to the BigQuery console and select your newly created project.
- In the navigation panel, select "Add Data" and then "Star a project by name".

  ## II. Design Thinking
  ### Step 1 - Empathize
| 5W1H                                                               |                                              |
| ------------------------------------------------------------------ |--------------------------------------------- |
| Who will be viewing this Dashboard?                                | Manager, production department, department in charge of importing raw materials<br> |
| If we had to choose only one key Stakeholder, who would it be?<br> | Department in charge of importing raw materials |
| What problem does this Dashboard solve?                            | Provides an overview of the situation of purchasing and selling raw materials and goods to serve the enterprise's production process. Identify suppliers that meet the standards of: quality, good price and on-time delivery.<br> |
| Describe the problem in one sentence                               | The purchasing situation with different suppliers to find a supplier that meets the standards of quality, price, and reasonable shipping time to meet the business's production process.<br> |
| When and where will Stakeholders view this Dashboard?<br>          | Dashboard can be view to monitor and evaluate factors serving the production process regularly, perhaps monthly or quarterly, from which to devise strategies to help fix, improve and enhance purchasing quality. Shop with better suppliers.<br> |
| Why do stakeholders need this Dashboard?<br><br>                   | This dashboard will synthesize data about product purchases from suppliers, prices, and supplier quality assessments so that it can be regularly monitored based on the standards set for purchases to help Evaluate and make decisions based on data quickly |
| How have stakeholders been achieving their goals so far?           | Focus on qualified suppliers. With suppliers that do not meet standards in terms of price, quality or delivery time: <br/> (1) Work again with these suppliers to find solutions to meet standards <br/>  (2) Search for new suppliers to replace <br/>|
<br/>

|Stakeholder Empathy Mapping                                 |                                                          |
| ---------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pains                                                      | - How do goods and raw materials meet the price and quality requirements? <br/>- What should be the solution when the supplier has not met one of the standards?                                                      |
| Thinking and feeling                                       | - What is the situation of buying and selling goods (price, quality) of the Enterprise? <br/>- Do the goods and raw materials meet the production process of the business? <br/>- What needs to be done to improve the purchase of goods and raw materials? <br/>- Are there any better suppliers on the market? <br/>         |
| Seeing                                                     | - Quantity of goods and prices imported from suppliers <br/>- Products with high failure rate <br/> - Suppliers that meet standards, suppliers that need to be re-worked or need to be replaced <br/>                                        |
| Saying and doing                                           | - I need to evaluate and work with unsatisfactory suppliers to achieve quality and time standards. <br/> - With the requirements for product supply standards, what factors do I need from a supplier? |
| Gains                                                      | With quality suppliers, the production process will be stable and can further improve quality and completion time.                             |

### Step 2 - Define POV
|                                      | NORTHSTAR METRIC                         |
|--------------------------------------|--------------------------------------|
| **What VALUE you want to measure?**  | Average Lead Time, Total Due, Total Order, Vendor'number, Order Status                              |
| **WHEN the value DELIVERY SUCCESS?** | The higher the reputation, the better the quality the vendors provide |
| **Northstar Metric Name**            | Vendor's number on Average Rating                              |
| **WHY do you choose this metric?**   | The vendor's reputation is an index that reflects the vendor's capacity in aspects such as: Selling price, product quality, service as well as delivery time to meet the set standards and requirements. |

<br/>

Dimension Point of View
|   View   | Why  | 
| -------- | -------- | 
| Overview | Overview of purchasing situation from vendors through number of orders, order fulfillment status, over the years |
| Vendor's Detail | Specifically reflects the number of products ordered by each vendor. Rank the reputation of each vendor, delivery time, number of goods imported, number returned due to unsatisfactory requirements |

### Step 3 - Ideate
Brainstorming
| Idea Name               | Layer 0 Dimension: Total Metrics              | Layer 1 Dimension: Breakdown by 1 Dimension                                   | 
|-------------------------|-----------------------------------------------|--------------------------------------------------------------------------------|
| Overview        | Total Order<br/>Total Due<br/>Order Status<br/>Order Qty<br/> | Total Order <br/> Total Due by Year <br/> Reject rate <br/>| 
| Vendor's Detail | AverageLeadTime <br/> Credit Rating | AverageLeadTime of each Vendor <br/> Credit Rating status |

<br/>

## III.Dashboard
### Data modeling
![image](https://github.com/Tien-Dung-86/PowerBI-Customer-Behaviour-Dashboard/blob/master/Visualization/1_Model_view.png)
### View 1: Overview
![image](https://github.com/Tien-Dung-86/PowerBI-Customer-Behaviour-Dashboard/blob/master/Visualization/2_Overview.png)
### View 2: Vendor's Detail
![image](https://github.com/Tien-Dung-86/PowerBI-Customer-Behaviour-Dashboard/blob/master/Visualization/3_Vendor_analysis.png)
