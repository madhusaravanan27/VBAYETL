# **VBAY Database Data Warehouse Project**

## **Project Overview**:

This project focuses on creating a Data Warehouse for the VBAY Database to streamline and optimize data management processes for key business areas such as:

- Ratings & Review Analysis
- Sales Process
- Location Analysis
- Bidding Process

By centralizing the data in a structured manner, the project provides insights to improve decision-making for VBAY. The project uses tools like DBT, Snowflake, and GitHub to create dimension and fact tables, facilitating a more efficient data analysis and reporting process.

## **Technologies Used**
- **DBT**: For data transformations, testing, and documentation in the ELT process.
  
- **Snowflake**: A cloud-based data platform used for SQL-based data warehousing.
  
- **GitHub**: For version control and collaboration on SQL queries and transformations.
  
## **Business Processes**

1.**Ratings and Review Analysis**:

Track the average ratings and reviews for buyers and sellers.

2.**Location Analysis:**

Analyze seller locations and item types based on zip codes.

3.**Sales Process:**
Manage data for items sold from the inventory.

4.**Bidding Process:**
Track the history of bids placed on items.

## **Bus Matrix**:

The Bus Matrix helps define the relationships between business processes and data dimensions. It helps organize data requirements for various business processes, allowing for easy integration between business processes and data dimensions.

## **Dimensional Model**:

The project uses a dimensional model to simplify database queries and optimize performance. This structure is designed to make querying more intuitive for end-users, especially for reporting and analysis tasks.

## **Dimension Tables**:
The following dimension tables were created to support the VBAY business processes:

- DIM_DATE:
Contains date-related attributes for time-based analysis.

- DIM_VB_ITEMS:
Contains information about items in the VBAY inventory.

- DIM_VB_USERS:
Contains details about buyers and sellers on the VBAY platform.

- DIM_VB_ZIP_CODES:
Stores geographical information to support location-based analysis.

**Fact Tables**:

The following fact tables were created to store quantitative data for VBAY's business processes:

- Location Analysis Fact Table:
  
Tracks location-based data and integrates with the DIM_VB_ZIP_CODES table.

- Sales Process Fact Table:
  
Stores data related to sales transactions from the VBAY platform.

- Bidding Process Fact Table:
  
Records the history of bids placed on VBAY items.

- Lineage Graph:
  
A lineage graph was created to visually represent the flow of data from the source to the final reporting layers. This graph helps track dependencies between tables and models.


