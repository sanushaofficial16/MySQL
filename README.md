Library System Management

This repository is created for Library System Management.

The database is named "library", and it consists of six tables: Branch, Employee, Books, Customer, IssueStatus, and ReturnStatus.

Branch Table:
This table stores information about the different branches of the library. It has four columns: Branch_no (Primary Key), Manager_Id, Branch_address, and Contact_no.

Employee Table:
This table stores information about the employees working in the library. It has five columns: Emp_Id (Primary Key), Emp_name, Position, Salary, and Branch_no (Foreign Key referencing the Branch_no column in the Branch table).

Books Table:
This table stores information about the books available in the library. It has seven columns: ISBN (Primary Key), Book_title, Category, Rental_Price, Status (indicating if the book is available or not), Author, and Publisher.

Customer Table:
This table stores information about the customers of the library. It has four columns: Customer_Id (Primary Key), Customer_name, Customer_address, and Reg_date (registration date).

IssueStatus Table:
This table stores information about the books issued to customers. It has five columns: Issue_Id (Primary Key), Issued_cust (Foreign Key referencing the Customer_Id column in the Customer table), Issued_book_name, Issue_date, and Isbn_book (Foreign Key referencing the ISBN column in the Books table).

ReturnStatus Table:
This table stores information about the books returned by customers. It has five columns: Return_Id (Primary Key), Return_cust (Customer ID), Return_book_name, Return_date, and Isbn_book2 (Foreign Key referencing the ISBN column in the Books table).

After creating the tables, all tables are displayed and the project requires writing SQL queries to perform various operations on the database. The queries are as follows:

* Retrieve the book title, category, and rental price of all available books.
* List the employee names and their respective salaries in descending order of salary.
* Retrieve the book titles and the corresponding customers who have issued those books.
* Display the total count of books in each category.
* Retrieve the employee names and their positions for the employees whose salaries are above Rs. 50,000.
* List the customer names who registered before 2022-01-01 and have not issued any books yet.
* Display the branch numbers and the total count of employees in each branch.
* Display the names of customers who have issued books in the month of June 2023.
* Retrieve book titles from the book table containing the word 'history'.
* Retrieve the branch numbers along with the count of employees for branches having more than 5 employees.
* Retrieve the names of employees who manage branches and their respective branch addresses.
* Display the names of customers who have issued books with a rental price higher than Rs. 25.
