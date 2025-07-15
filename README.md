# Food Delivery App - Database Design

## Overview
The goal of this database is to represent the essential structure of a food delivery system in a normalized and relational format. It includes support for multiple restaurants, dynamic menus, customer orders, and delivery addresses.

## Features
- Customer registration and profile information  
- Restaurant listings and contact details  
- Menu items offered by multiple restaurants  
- Shopping cart functionality with item quantities  
- Order tracking and status  
- Customer address storage for deliveries  

## Main Tables

- **Customer**: Stores customer personal and contact details  
- **Restaurant**: Contains restaurant information including cuisine type and average price  
- **MenuItem**: Stores food item details like name, price, and description  
- **Restaurant_Menu**: Many-to-many mapping of menu items to restaurants  
- **Cart**: Represents customer carts with total amount  
- **Cart_Item**: Connects individual menu items to a cart with quantity  
- **Orders**: Tracks placed orders, linked to customer and cart  
- **Customer_Address**: Stores customer delivery addresses  

## Database Design Goals
- Use foreign keys to establish proper relationships between tables  
- Enforce data consistency using appropriate constraints  
- Keep the schema normalized and modular for scalability  
