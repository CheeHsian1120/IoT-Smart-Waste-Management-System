# IoT Smart Waste Management System
![Data Modeling](https://img.shields.io/badge/Data_Modeling-Conceptual_%7C_Logical-0052CC?style=for-the-badge)
![Oracle Data Modeler](https://img.shields.io/badge/Oracle_Data_Modeler-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![Database](https://img.shields.io/badge/Database_Design-3NF_Normalization-4EA94B?style=for-the-badge)
![Draw.io](https://img.shields.io/badge/Draw.io-F08705?style=for-the-badge&logo=diagramsdotnet&logoColor=white)

## 📌 Executive Summary
This project focuses on the end-to-end database architecture for **Clear Away (CA)**, a logistics enterprise introducing an IoT-driven "Pay-As-You-Dump" (PAYD) program for local government authorities. 

The system tracks RFID-enabled smart wheelie bins, manages municipal waste collection contracts, and calculates dynamic billing based on waste type and weight[cite: 9]. The project demonstrates the complete database design lifecycle, from gathering business requirements to generating a robust Oracle relational schema[cite: 9].

## 🛠️ Key Technical Features
* **Rigorous Normalization:** Processed raw, unnormalized collection reports through 1NF, 2NF, and ultimately to **Third Normal Form (3NF)**, effectively eliminating data anomalies and redundancy.
* **Conceptual & Logical Modeling:** Engineered a comprehensive Entity-Relationship Diagram (ERD) utilizing Crow's Foot notation. Translated the conceptual design into a production-ready logical model using **Oracle SQL Developer Data Modeler**.
* **Strategic Architecture Decisions:** Implemented surrogate keys (e.g., `prop_id`, `collrun_id`, `cb_num`) to optimize database efficiency, resolve converging foreign keys, and streamline complex natural key combinations.
* **Data Integrity & DDL Generation:** Generated strict Data Definition Language (DDL) scripts enforcing business rules through `UNIQUE` constraints, `CHECK` constraints (e.g., bin replacement reasons, road types), and foreign key relationships.

## 📊 Database Architecture Visualization
### 1. Conceptual Model (ERD)
`![Conceptual Model](link_to_ca_conceptual.png)` 
*(Upload your `ca_conceptual.pdf` as an image and link it here)*

### 2. Logical Model
`![Logical Model](link_to_ca_logical.png)`
*(Upload your `ca_logical.pdf` as an image and link it here)*

## 📁 Repository Structure
* `ca_conceptual.pdf` - The foundational Entity-Relationship Diagram outlining business entities and cardinalities.
* `ca_normalisation.pdf` - Step-by-step mathematical breakdown of data dependencies from UNF to 3NF.
* `ca_logical.pdf` - The refined relational model depicting foreign keys, data types, and structural integrity.
* `ca_assumptions.pdf` - Documentation of strategic engineering decisions and business logic assumptions.
* `ca_schema.sql` - The executable Oracle DDL script generated for database deployment.
* `ca_schema_output.txt` - Verification log confirming the successful creation of all tables and constraints.

## 👨‍💻 Author
**Tay Chee Hsian** 
