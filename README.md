# E-commerce-Back-End

[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Project Summary
To build the back end for an e-commerce web application that can be used by an internet retail company to enable them to 
compete with other e-commerce companies. The project requires modifying starter code that has been provided, and configuring 
a working Express.js API to use Sequelize to interact with a MySQL database named 'ecommerce_db'. To include a walkthrough video 
that demonstrates the functionality of the e-commerce back end in accordance with the requirements set out in the acceptance criteria. 

## Video

The following video shows the user flow through the application., including all prompts and updated tables:

https://drive.google.com/file/d/1w-9EKvhECklP3dMO_Rd_6PBOrikpDluy/view


## Packages Used

- Node.js: Executes JavaScript code outside a web browser.
- MySql: A relational database management system based on structured query language (SQL).    
- Sequelize: A modern TypeScript and Node.js Object Relational Mapping (ORM) that offers solid transaction support.
- Express.js: Node.js web application framework providing broad features to build web & mobile application.
- Insomnia API Design Platform: A collaborative API client and Design Tool.
- .env: Used to store environment variables data used by the operating system and other programs (DB_Name, DB_User, DB_PW).

## E-commerce Back End

The E-commerce Back End web application is set-up and synced to the database at the command-line application (terminal).  Once
the program is running the business owner or other user is able to view, create, update or delete data in the **ecommerce_db**
database using the **Insomnia API development platform**. The information being stored, viewed and modified consists of Categories, Products and Tags. 
These are stored within the E-commerce Back End application as objects that contain properties. 

***Note***: *A description of how to use the completed web application appears in the 'Usage' section below.*

## Project Description

The objective of this project was not just to produce an E-commerce Back End, it was to effectively create an application in which
**Node.js**, **SQL**, **Sequelize** and **Express.js** could connect and work together in sync. In addition that API routes could 
be either accessed, viewed or manipulated using the **Insomnia API development platform**.

Even though a starter code was provided the project still required a considerable amount of careful coding that had to be 
'well thought out' to enable the whole application to work.

The files that needed to be created and/or coded were as follows:
- .env
- models
  - Category.js
  - index.js
  - Product.js
  - ProductTag.js
  - Tag.js
- routes
  - category-routes.js
  - product-routes.js
  - tag-routes.js
- server.js required additional coding to be added.   
## Installation 

To install this application, simply download from Github.

## Usage

To create the developmental database seeded with test data, at the command-line the user must enter the following commands in order:

1. At server.js right click and select Open in Integrated Terminal,
2. At $ prompt type in mysql -u root -p,
3. At Enter password prompt type in password,
4. At mysql prompt type in source db/schema.sql,
5. At mysql prompt type in quit,
6. At $ prompt type in *npm run seed*.

Once completed successfully, to invoke the application the user enters the command *NPM run start*

**Insomnia**

Within the Insomnia window by entering the correct port and pathway functions are run by accessing the following routes:

- *category-routes.js* 
- *product-routes.js* AND
- *tag-routes.js*. 

The user chooses the requests type from a drop down menu and has the option to select all records or narrows the search by adding the 'id' to the pathway.

The image below shows a request to GET (display) all product records:

![image](https://user-images.githubusercontent.com/115671306/222353106-97285291-d7d4-4c61-a591-a09566ae4502.png)

For this application, the following explanation of Request types apply:

- **GET:** Display information from the route selected
     - All or a single record.
- **POST:** Creates a new record (Category, Product or Tag).
- **PUT:** Updates a record.
- **DELETE:** Deletes a record.

If an error message is returned the user may need to re-enter the command *npm run start*

## Licence

MIT