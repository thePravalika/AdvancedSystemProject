# AdvancedSystemProject
An Online Bookstore - using  SpringBoot and Microservices

The entire application consists of two portals: - 1) adminportal and 2) bookstore

The adminportal is responsible for maintaining the inventory of products(books), orders placed by the users, 
tracking the back orders made by the users and updating the inventory based on the product quantity requested by the customers 
(both in case of normal orders and backorders).

The bookstore portal provides the functionality for the users to get registered with the bookstore website and 
can perform all the intended operations. Some of the functionalities include browsing the bookshelf, updating the account details,
adding items to the cart. The users also get notification emails upon successful checkout i.e., Order confirmation information,
when new stocks of their interest arrive, and also when their order gets cancelled by bookstore admin.


Technologies: - 
•	System Platform: - Mysql, Apache Tomcat.
•	Front end development: - HTML5, CSS3, JavaScript, Bootstrap, jQuery, Ajax.
•	Back end: - Spring Boot, Spring MVC, JPA, Hibernate, Spring Thymeleaf.
•	Design Patterns: - Strategy Pattern, MVC Pattern.
•	Programming Language: - Core Java.

Non-Functional Requirements: - Security (Spring Security), Logging etc.


Functional Requirements of adminportal: - 
1)	Admin can perform all the CRUD (creation, insertion, update and deletion of products) operations of the book.
2)	Admin can view the list of orders placed by the bookstore users.
3)	Admin can cancel an order placed within 24 hours of timeframe, when required.
-	In this case, the user ordered stock will be added back to the bookstore repository.
-	A confirmation email will be sent to the user about money refunding process.
4)	Admin can track the deficit of products by maintaining list of backorders.
-	When new stock of deficit/required stock arrives, the intended quantity will be reserved for the user requested and rest of the stock will be added to the repository.
5)	Admin can search the list of backorders made by users between a particular time frame.
-	Admin retrieves the information by entering start and end dates.
6)	Admin can search the orders made by a particular customer by entering username of customer.
7)	Admin can search particular book by entering the book title.

Functional Requirements of bookstore portal: - 
1)	User can create an account by providing username and email address.
-	The sign-up instructions will be sent to their email along with providing 16-digit password token.
2)	Registered users can login into application by validating against username and password.
-	Users can choose “Forgot Password” when required, an email with instructions will be sent to the user.
3)	Registered users can update account details like name, email address, password, username etc.
4)	Registered users can add default shipping address and payment method.
5)	Users can search for particular product (browse the bookshelf) by entering book title.
6)	Registered users should be able to place any number of orders.
7)	Registered users can update the cart (adding, deleting, updating the product quantity) any number of times before proceeding for the checkout.
8)	Registered users pay for the products in the cart by providing card details.
9)	Registered users get a confirmation email upon placing orders along with providing shipping details.
10)	 Registered users get a notification email if the new stocks of their interest were added.
11)	 Registered users get a confirmation email if their order got cancelled.



