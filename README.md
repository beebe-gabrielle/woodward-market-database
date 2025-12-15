## End‑to‑End SQL Project: Schema Design, Cleaning, and Business Analysis

## Project Overview & Context
This project uses a fictional retail/e‑commerce dataset I generated using AI to simulate operations at a fictional Detroit‑inspired local retailer, "Woodward Market & Co". I've generated the dataset to reflect the inconsistent data challenges businesses face in real life.

<img width="828" height="230" alt="image" src="https://github.com/user-attachments/assets/a59f31f0-e64a-4c9d-afcf-82da84f7a63b" />


**Objective:** The goal of this project is to design a normalized SQL schema, clean messy data, and generate actionable insights. By enforcing referential integrity and applying advanced SQL techniques, the project demonstrates how raw, inconsistent data can be transformed into reliable business intelligence.

**Business Problem:** Retail businesses often struggle with poor data quality. These issues make it difficult to track customer behavior, properly monitor inventory, and measure product performance. Without clean data, decision‑making is slow and error‑prone.

**Business Value:** This project shows how SQL can solve those problems by:
*  Enforcing data integrity with primary and foreign keys.
*  Cleaning and standardizing messy data for accurate reporting.
*  Producing insights into customer lifetime value, category performance, and inventory shortages.

## 1. Creating Database Schema:
This dataset is structured into multiple relational tables including order_items, orders, inventory, products, and customers. I designed an Entity Relationship Diagram (ERD) to map out the cardinality between these tables, guiding my schema creation process and ensuring proper use of primary and foreign keys.

<img width="866" height="536" alt="image" src="https://github.com/user-attachments/assets/e6797eb5-075f-491c-afa7-f0c4a77d7bb9" />

  
## 2. Data Cleaning:
The first step in preparing the dataset for analysis involved a thorough data cleaning process. To illustrate, a snippet of the original data from the customers table is included below, showing the raw, unprocessed entries.
</p>
<img width="1102" height="230" alt="image" src="https://github.com/user-attachments/assets/f8b37fa5-9ffa-4601-a47b-2faa9485b107" />
</p>
To identify missing values, each column in the customers table was explicitly checked for NULL values. This allowed for precise handling of missing data based on the role and importance of each field
</p>
<img width="551" height="321" alt="image" src="https://github.com/user-attachments/assets/2a9322a6-80a4-418a-80c7-f34b41df59e2" />
</p>
<img width="981" height="50" alt="image" src="https://github.com/user-attachments/assets/f0b76d95-857a-489f-af47-9d071e3eddc8" />
</p>
Fixing NULL, empty, or missing values
Normalized 'state' to have code abbreviations:
</p> 
<img width="610" height="192" alt="image" src="https://github.com/user-attachments/assets/e7ac98cb-b436-40f4-b418-7942097e7aea" />
</p>
Normalized 'phone' into XXX-XXX-XXXX format:
</p>
<img width="612" height="423" alt="image" src="https://github.com/user-attachments/assets/bfcc3d7f-7ce7-4300-9746-c3a4cf027772" />
</p>
Normalized 'zip_code' to store only the first 5 numbers:
</p>
<img width="687" height="62" alt="image" src="https://github.com/user-attachments/assets/603b1e44-55da-4bc3-8629-5bb7a4714358" />
</p>
The resulting table with clean data:
</p>
<img width="1046" height="233" alt="image" src="https://github.com/user-attachments/assets/49c6c4bb-cbfe-4104-96a8-5564ef228056" />
</p>
<i> Additional cleaning scripts for other tables are included in the sql_scripts folder for reference.

## 4. Key Insights & Visualizations
This section is crucial for showcasing your findings. Display key visuals (if hosted elsewhere, like a dashboard) and explain what they represent.

*   **Insight 1:** Briefly explain the insight and its relevance. Include a link to the relevant visualization or a static image if necessary.
*   **Insight 2:** Repeat for other key insights.

## 5. Recommendations & Conclusion
Officially answer the questions posed in the problem statement. Provide actionable business solutions based on your insights.

*   **Recommendation 1:** Suggest a concrete business action based on your findings.
*   **Recommendation 2:** Suggest another action.
*   **Conclusion:** Summarize the overall project outcome and the value delivered.


