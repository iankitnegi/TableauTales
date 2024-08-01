# [Tableau Ultimate Full From Zero to HERO](https://youtu.be/K3pXnbniUcM?si=X2iYF8-ogMRQxBP8)

### Data normalization is the process of organizing structured data in a database to reduce redundancy and improve data integrity.  
- Purpose: Data normalization ensures consistency across applications and improves query performance by reorganizing data to remove unstructured or redundant information.
- Techniques: It involves decomposing tables into smaller, related tables and assigning primary keys to establish relationships.
- Benefits:
  - Reduced Redundancy: Normalized data eliminates duplicate entries, leading to more efficient storage.
  - Improved Integrity: Ensures data consistency and accuracy.
  - Better Query Performance: Simplifies data retrieval and analysis.


## Basics Data Modeling
Star Schema: Star schema is the simplest method for arranging data in a data warehouse. It contains a fact table at the center connected to dimension tables around it. Star schema is most effective for quick and simple data query execution.   
Snowflake Schema: Snowflake schema is a more complex method of storing data in which fact tables, dimension tables and sub-dimension tables are connected through foreign keys. Snowflake is most effective for in-depth data query analyses.

## Logical & Physical Layers
1. Physical Layer: The Physical Layer represents the raw data sources and how they are combined. It includes:
   - Join: Combines two tables (A and B) based on a common field.
   - Union: Stacks two tables (A and B) vertically, combining rows from both tables.
2. Logical Layer: The Logical Layer abstracts the physical data into logical tables, which can be used for analysis and visualization.
   - Join in Logical Layer: The result of a physical join is presented as a new combined logical table (AB).
   - Union in Logical Layer: The result of a physical union is presented as a new combined logical table (AB).
   - Relationship: Establishes a relationship between two logical tables (A and B) without combining them into a single table. This allows for more flexible data modeling.
### Data Profiling is the process of examing and investigating the data to understand the content of the tables.
3. Visualization: This layer represents how the data is visualized and analyzed.
   - Visualization with Combined Logical Table: Data from the combined logical table (AB) is visualized, showing data from both tables A and B.
   - Visualization with Related Logical Tables: Data from the related tables (A and B) is visualized, maintaining the relationship defined in the logical layer.
   - Blending: Combines data from primary and secondary data sources for visualization, useful when data sources cannot be joined directly.
  
**Always prefer Relationships & then Data Blending at Viz Level**

Key Concepts:
- Data Sources (A and B): The origin points of data that can be combined through joins or unions.
- Join: A method to combine data from two tables based on a related column.
- Union: A method to append data from one table to another.
- Relationship: Links two tables based on common fields without merging them.
- Blending: Integrates data from different sources in the visualization layer. {BY DEFAULT: LEFT JOIN, CAN'T CHANGE}
