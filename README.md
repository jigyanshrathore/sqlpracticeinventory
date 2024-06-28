# sqlpracticeinventory
The SQL commands provided outline the creation of a relational database schema tailored for a comprehensive retail management system. 
The provided SQL commands collectively establish a relational database schema designed for a retail management system. It includes tables for managing brands, inventory users, product categories, products, stores, pricing, customer transactions, and invoicing. Data insertion operations populate these tables with sample records for brands like Apple and Nike, various product categories, store locations, customer details, selected products, and transactional information. The system facilitates inventory management, sales tracking, and customer interaction through robust data integrity measures such as primary and foreign keys. Stored procedures and cursors enhance functionality for tasks like stock verification and data retrieval, ensuring efficient operations within the retail environment.

Here is a summary of the output from the SQL commands and interactions provided:

1. **Database Schema Creation**:
   - Tables created include `brands`, `inv_user`, `categories`, `product`, `stores`, `provides`, `customer_cart`, `select_product`, `transaction`, and `invoice`.
   - Primary keys (`bid`, `user_id`, `cid`, `pid`, `sid`, `cust_id`, `id`, `item_no`) and foreign keys (`cid`, `bid`, `sid`, `user_id`, `cart_id`, `pid`, `transaction_id`) are defined to maintain data integrity.

2. **Data Insertion**:
   - Records inserted into tables:
     - `brands`: Apple, Samsung, Nike, Fortune
     - `inv_user`: Executive users with roles such as admin, manager, and accountant
     - `categories`: Electronics, Clothing, Grocery
     - `stores`: Ram Kumar in Katpadi Vellore, Rakesh Kumar in Chennai, Suraj in Haryana
     - `product`: Various products like iPhone, Airpods, Smart Watch, Air Max, Refined Oil with details like stock, price, and added date
     - `provides`: Relationships established between brands and stores with associated discounts
     - `customer_cart`: Records for customers like Ram, Shyam, Mohan with their contact details
     - `select_product`: Products selected by customers with quantities specified
     - `transaction`: Transactions recorded with details including total amount, payments made, dues, GST, discounts, and payment methods
     - `invoice`: Items listed on invoices with quantities and net prices linked to transactions

3. **Stored Procedures and Cursors**:
   - **Stored Procedures**: Implemented for functions like `check_stock` to verify product availability based on stock levels.
   - **Cursors**: Used to iterate through product details for listing and reporting purposes.

4. **Functionality Overview**:
   - **Inventory Management**: Tracks product availability (`p_stock`) and manages stock levels across stores.
   - **Sales and Invoicing**: Facilitates customer transactions, generates invoices (`invoice`), and calculates total amounts, dues, and discounts.
   - **User Management**: Defines roles (`user_type`) for users (`inv_user`) accessing the system.

5. **Overall System Purpose**:
   - Provides a comprehensive backend system for retail operations, managing inventory, sales, and customer interactions efficiently.
   - Supports multiple stores (`stores`), brands (`brands`), and product categories (`categories`), ensuring robust data management and transaction handling.

