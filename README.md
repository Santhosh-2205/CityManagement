# City Management Database Project

Welcome to the City Management Database project repository. This project was developed as part of a DNA (Data and Applications) course and is structured into four phases, focusing on different aspects of database design, normalization, implementation, and functional requirements.

## Phase 1: Requirements and Design
### Project Overview
The primary purpose of the City Management Database is to centralize, manage, and analyze financial data for cities, enabling government officials, policymakers, and other stakeholders to make informed decisions about resource allocation
### Requirements Document
The detailed requirements for database design and functional operations are documented in [phase1_Requirements.pdf](phase1_Requirements.pdf).

## Phase 2: Entity-Relationship (ER) Diagram
### ER Diagram Design
An Entity-Relationship (ER) diagram is designed based on the requirements document to visualize the data model.
### ER Diagram Document
The ER diagram is detailed in [phase2_ER.pdf](phase2_ER.pdf).

## Phase 3: Relational Model and Normalization
### Relational Model Conversion
The ER model is converted into a relational schema and normalized up to the Third Normal Form (3NF) to eliminate redundancy and improve data integrity.
### 3NF Document
Details of the relational model in 3NF can be found in [phase3_Normalization.pdf](phase3_Normalization.pdf).

## Phase 4: Database Implementation and CLI
### Database Implementation
The relational schemas are implemented in MySQL, and the database is populated with initial data.
### Command Line Interface (CLI)
A Python3-based Command Line Interface (CLI) `cli.py` is developed to interact with the database, fulfilling the functional requirements specified earlier. The CLI provides the following functionalities:
- Detailed instructions on using the CLI are available in [phase4_Report.pdf](phase4_Report.pdf).
- A demonstration video ([Demo.mp4](Demo.mp4)) showcases the CLI in action.
  
## Source Code
The `source_code` directory contains:
- `cli.py`: Command Line Interface implementation in Python3.
- `Data.sql`: SQL script to initialize the database with sample data.

## Running or Using

#### Setting Up the Database
1. **Create Database:**
   - Open MySQL and create a database named `cm` (or any preferred name).

2. **Update Credentials in `cli.py`:**
   - Open `cli.py` and update lines 9 and 10 with your MySQL username and password:
     ```python
     USERNAME = "your_mysql_username"
     PASSWORD = "your_mysql_password"
     ```

3. **Modify Database Name in `cli.py` and `Data.sql`:**
   - If you chose a database name other than `cm`, update the following:
     - In `cli.py`, change line 430:
       ```python
       db = "cm"
       ```
     - In `Data.sql`, change line 1 to use your chosen database:
       ```sql
       USE cm;
       ```
#### Running the CLI
- Navigate to the `source_code` directory and run the CLI using Python3:
  ```bash
  python3 cli.py
Once cli.py is running, follow the instructions displayed on the screen to interact with the database and execute various commands as per the functionalities provided.

