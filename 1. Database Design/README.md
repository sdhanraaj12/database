# Database Design
## What is a Data Warehouse?
data warehouse is a collection of data. It has the following properties:

- **Subject-oriented**: A data warehouse should contain information about a few well-defined subjects rather than the enterprise.
- **Integrated**: A data warehouse is an integrated repository of data. It contains information from various systems within an organisation.
- **Non-volatile**: The data values in a database cannot be changed without a valid reason.
- **Time-variant**: A data warehouse contains historical data for analysis.

## Structure of a Data Warehouse

Dimensional modelling 
- Dimensions : the metadata (that is, data explaining some other data) attached to the fact variables. 
- Facts : the numerical data in a data warehouse 

Both facts and dimensions are equally important for generating actionable insights from a data set.

## Star Schema
A schema is an outline of the entire data warehouse. It shows how different data sets are connected and how the different attributes of each data set are used for the data warehouse.

**There are four types of schemas** are available in data warehouse. Out of which the star schema is mostly used in the data warehouse designs. The second mostly used data warehouse schema is snow flake schema. We will see about these schemas in detail.

1. Star Schema:

   A star schema is the one in which a central fact table is sourrounded by denormalized dimensional tables. A star schema can be simple or complex. A simple star schema consists of one fact table where as a complex star schema have more than one fact table.
   
    <p align="center">
      <img width="460" height="300" src="https://1.bp.blogspot.com/-v6KdFsvuzyM/XOlvM-gm4zI/AAAAAAAAAM8/Axqw6P-SA9EEf7z6_cwVve7pV33ePAMcgCLcBGAs/s1600/stare.jpg">
    </p>

2. Snow Flake Schema:

   A snow flake schema is an enhancement of star schema by adding additional dimensions. Snow flake schema are useful when there are low cardinality attributes in the dimensions.
   
   <p align="center">
      <img width="460" height="300" src="https://1.bp.blogspot.com/_pjSOGJIjDMo/S1w_JRMx3XI/AAAAAAAAADQ/J6cKyxJiwbM/s1600/Snowflake-schema.png">
   </p>



3. Galaxy Schema:

    Galaxy schema contains many fact tables with some common dimensions (conformed dimensions). This schema is a combination of many data marts.
    
    <p align="center">
      <img width="460" height="300" src="https://1.bp.blogspot.com/_pjSOGJIjDMo/S1w_SAaqJBI/AAAAAAAAADY/_kYiR3xwbCQ/s1600/galaxy.bmp">
    </p>




4. Fact Constellation Schema:

   The dimensions in this schema are segregated into independent dimensions based on the levels of hierarchy. For example, if geography has five levels of hierarchy like teritary, region, country, state and city; constellation schema would have five dimensions instead of one.
    <p align="center">
      <img width="460" height="300" src="https://media.geeksforgeeks.org/wp-content/uploads/factnew.jpg">
    </p>
    
## OLAP vs OLTP
<p align="center">
      <img width="460" height="300" src="/assets/diff.png">
</p>
