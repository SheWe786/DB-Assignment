1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
   
Answer:- 

Nature of Relationship:
The relationship between "Product" and "Product_Category" entities is one of association, where each product is categorized into one specific product category.
This relationship allows for the organization and classification of products based on shared characteristics or attributes.

One-to-Many Relationship:
Typically, there exists a one-to-many relationship between "Product_Category" and "Product".
This means that each product category can have multiple products associated with it, but each product can only belong to one category at a time.

2. How could you ensure that each product in the "Product" table has a valid category assigned to it?
   
Answer:-
   
1:- Utilize foreign key constraints in the database schema. By defining a foreign key relationship between the "Product" and "Product_Category" tables, you enforce referential integrity. This ensures that every value in the category_id column of the "Product" table must correspond to a valid primary key value in the category_id column of the "Product_Category" table.
2:- Implement data validation rules within the application logic. Before inserting or updating a product record in the "Product" table, validate that the associated category exists in the "Product_Category" table. If the category does not exist, prevent the operation or prompt the user to select a valid category.
