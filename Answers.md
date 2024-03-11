1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

One-to-Many Relationship - Product_Category to Product:
In the database schema, a one-to-many relationship exists between the "Product_Category" table, where each category can be associated with multiple products, and the "Product" table, where each product is uniquely linked to one category through the "CategoryID" foreign key.

2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

To ensure that each product in the "Product" table has a valid category assigned to it, you can use a foreign key constraint.
This can be achieved:
(a). When creating the "Product" table, specify that the "CategoryID" column is a foreign key referencing the "CategoryID" column in the "Product_Category" table.
(b). Declare the "CategoryID" column in the "Product" table as NOT NULL to ensure that every product must have a valid category.