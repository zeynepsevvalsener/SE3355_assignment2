Project Title: Flask E-Commerce Web Application
Overview
This project is a simple e-commerce platform built using Flask, SQLite, and Jinja2 templates. It provides functionality for listing, searching, and viewing details of products based on categories and other attributes. The application is designed for learning purposes and can be extended for real-world use cases.
 
Data Model
The application uses an SQLite database with a single primary table, products. The schema for the products table is as follows:
Column Name	Data Type	Description
ad_no	INTEGER	Primary key. Auto-incremented unique identifier.
title	TEXT	Title of the product. Cannot be null.
description	TEXT	A brief description of the product.
price	REAL	Price of the product in the local currency.
city	TEXT	City where the product is available.
image_url	TEXT	Path or URL to the product's image.
category	TEXT	Category of the product (e.g., "Clothing").
 
Assumptions
1.	Product Data:
o	All products have a unique ad_no.
o	Product prices are provided in a consistent currency (e.g., USD, EUR).
o	Each product belongs to one category, but the system can be extended to support multiple categories per product.
2.	Data Validation:
o	Data validation is assumed to be handled on the front-end or via form validation in Flask forms.
3.	Database:
o	The SQLite database is used for simplicity. It can be migrated to a relational database like MySQL or PostgreSQL for larger-scale projects.
4.	Static Files:
o	All images are stored in the static/images folder, and the image_url column in the database points to this path.
o	CSS styles are included in the static/css directory.
5.	Search Functionality:
o	The search functionality matches products by title, description, or category.
 
Features
1.	Home Page:
o	Displays a list of all products categorized by popularity or category.
2.	Search Page:
o	Users can search for products by entering keywords.
o	Results are displayed in a grid layout with product images, descriptions, and prices.
3.	Detail Page:
o	Displays full product details, including an image, description, price, and category.
o	Includes breadcrumbs for easy navigation.
4.	Database Management:
o	Products can be added, updated, or deleted from the database.

