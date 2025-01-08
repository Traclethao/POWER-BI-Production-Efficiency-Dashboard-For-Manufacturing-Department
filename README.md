# Production Efficiency Dashboard For Production Department
Using Power BI to visualize dashboards about the business's production efficiency 

## **I. Introduction**

### **1. Situation**

- **AdventureWorks database** of a fictitious bicycle manufacturer - Adventure Works Cycles contains **Manufacturing**.
- The Production Department is responsible for receiving production requests from the Company's planning department. After the Purchasing Department places orders and imports raw materials to the warehouse, production begins.
- According to the plan, when production is completed, the products will be stored in many different locations for convenient storage and distribution to customers. The production completion time may not completely match the plan. During the warehouse inspection process, there is a possibility that the goods will be damaged, and will be eliminated to ensure that only quality products are stored for sale.
- The dataset includes a **dim table** containing information about product and warehouse location, including fields of **product** information (ID, name, category, and subcategory, BOM, takt time) and information related to the **warehouse location** (LocationID, name, CostRate, availability).

### **2. Business Questions**

- Create an Operation Dashboard for managers that displays production yield, scrapped ratio, on time rate, average units produced, good units produced, throughput, cycle time (hours), takt time (hours), and BOM.

### **3. Data Model**

From the company's data dictionary I did data modeling.

![Data Modeling](https://github.com/user-attachments/assets/a9861a44-640a-4ac6-b192-960ced3f8fca)

## **II. Design Thinking Method**

**Here are the five steps of design thinking:**

### **Step 1 - Empathize**

![Stage 1](https://github.com/user-attachments/assets/2f444ce7-7165-41ee-be5e-e0ad7501d264)

### **Step 2 - Define**

![Stage 2](https://github.com/user-attachments/assets/21686fd1-846b-4d71-9482-782f304f3f6c)

### **Step 3 - Ideate**

![Stage 3](https://github.com/user-attachments/assets/3c330a87-3b64-4aae-870d-eba00034f760)

### **Step 4 - Prototype**

![Stage 4](https://github.com/user-attachments/assets/2a5b3453-1d2e-425a-9aa4-256b1a1caf00)

### **Step 5 - Review**

![Stage 5](https://github.com/user-attachments/assets/1073f2d1-a8fd-4537-a8c8-d9282d639796)

## **III. Visualization & Insights**
### **1. Production Efficiency**

![Production Efficiency](https://github.com/user-attachments/assets/3a79bf10-d90d-4907-9f08-4a4b19b343aa)

### **2. Information Per Product**

![Information Per Product](https://github.com/user-attachments/assets/96ff6720-0c37-4802-93c3-c366f7964990)
