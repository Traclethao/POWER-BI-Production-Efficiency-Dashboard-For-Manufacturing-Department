# Production Efficiency Dashboard For Production Department
Using Power BI to visualize dashboards about the business's production efficiency 

## **I. Introduction**

### **1. Situation**

- **AdventureWorks database** of a fictitious bicycle manufacturer - Adventure Works Cycles contains **Manufacturing**.
- The Production Department is responsible for receiving production requests from the Company's planning department. After the Purchasing Department places orders and imports raw materials to the warehouse, production begins.
- According to the plan, when production is completed, the products will be stored in many different locations for convenient storage and distribution to customers. The production completion time may not completely match the plan. During the warehouse inspection process, there is a possibility that the goods will be damaged, and will be eliminated to ensure that only quality products are stored for sale.
- The dataset includes a **dim table** containing information about product and warehouse location, including fields of **product** information (ID, name, category, and subcategory, BOM, takt time) and information related to the **warehouse location** (LocationID, name, CostRate, availability).

### **2. Business Questions**

- Create an Operation Dashboard for managers that displays production yield, scrapped ratio, on time rate, average units produced, good units produced, throughput, cycle time (hours), and BOM.

### **3. Data Model**

From the company's data dictionary I did data modeling.

![Data Modeling](https://github.com/user-attachments/assets/a9861a44-640a-4ac6-b192-960ced3f8fca)

## **II. Design Thinking Method**

**Here are the five steps of design thinking:**

### **Step 1 - Empathize**

![Stage 1](https://github.com/user-attachments/assets/b433e242-96f5-4c02-bd8e-7d22e376e08d)

### **Step 2 - Define**

![Stage 2](https://github.com/user-attachments/assets/21686fd1-846b-4d71-9482-782f304f3f6c)

### **Step 3 - Ideate**

![Stage 3](https://github.com/user-attachments/assets/8286ddf7-5a3f-499d-a023-92b62cfd0274)

### **Step 4 - Prototype**

![Stage 4](https://github.com/user-attachments/assets/2a5b3453-1d2e-425a-9aa4-256b1a1caf00)

### **Step 5 - Review**

![Stage 5](https://github.com/user-attachments/assets/1073f2d1-a8fd-4537-a8c8-d9282d639796)

## **III. Visualization & Insights**
### **1. Production Efficiency**

![Production Efficiency](https://github.com/user-attachments/assets/cad1b7bc-d564-482e-b8c0-d4541c3208f0)

- **Production Yield**: This is the percentage of products that are produced without defects in relation to the total number of products manufactured. High yield indicates an efficient production process.

- **Scrapped Ratio**: This is the proportion of products that are discarded due to defects or failures. Lower scrapped ratios are preferred as they indicate less waste and higher efficiency.

- **On-Time Rate**: The percentage of orders completed and delivered on time, relative to the total orders. This reflects the reliability and punctuality of the manufacturing process.

- **Average Units Produced**: This is the average number of units produced over a specific period, which helps in measuring the consistency and scale of production.

- **Good Units Produced**: The total number of units that meet quality standards without requiring rework or being scrapped.

- **Throughput**: This is the rate at which products are produced and completed within a given period, reflecting the efficiency of the production process. Tracking throughput to understand production capacity and planning for scale. 

**=> Insight:**
    - Production Yield and Scrapped Ratio are good.
    - **On Time Rate** of 42% in 2013 is low => the company needs to improve this ratio by reviewing the production time planning accordingly. **Switch to information per product dashboard to see the specific production time of each product to plan production.**

### **2. Information Per Product**

![Information Per Product](https://github.com/user-attachments/assets/f3de3fc8-fc13-4218-9863-6e3453864670)

- **Cycle Time**: The total time taken to produce a unit from start to finish, including processing, waiting, and transport times. Monitoring cycle time helps in identifying bottlenecks and streamlining the process. 

- **BOM (Bill of Materials)**: A comprehensive list of materials, components, and instructions required to construct, manufacture, or repair a product. It includes quantities, prices, and detailed information about each part.

**=> Insight:**
   - The company is calculating the **planned production time for the entire order to be 11 days**, **but** each order has a different quantity and the **average actual production time is 12 days**.
   - Looking at the ActualProductionTime VS PlannedProductionTime by WorkOrderID chart, it can be seen that **each order with a different quantity will have a different actual production time**.
**=> Recommend that the company calculate the planned production time based on the quantity of products per order.**

