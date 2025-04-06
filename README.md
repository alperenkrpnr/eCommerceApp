# E-Commerce Web Application

## Overview
This project is an e-commerce web application developed as part of the *Cloud Computing* course at **Middle East Technical University**. The application allows users to browse, search, filter, and sort products; view product details including ratings and reviews; and leave their own ratings and reviews. Additionally, admin users can add or remove products and users.

## Deployment
The application is deployed on **Vercel** as a Platform-as-a-Service (PaaS).

**Deployment URL:** [https://e-commerce-app-wine-chi.vercel.app/]

## Technologies Used

- **Programming Language:** Python  
  Chosen for its readability, extensive libraries, and rapid development capabilities.

- **Web Framework:** Flask  
  Flask’s minimalist and flexible design allows for quick prototyping and modular development.

- **Database:** MongoDB Atlas (NoSQL)  
  MongoDB’s dynamic schema makes it ideal for managing product and user data with flexibility.

- **Frontend:** HTML, Bootstrap 5, and Font Awesome  
  Bootstrap 5 provides a responsive, modern design while Font Awesome supplies the necessary icons.

- **Authentication:** flask-login  
  Used for managing user sessions and authentication.

- **Database Integration:** flask-pymongo  
  Facilitates seamless interaction between Flask and MongoDB.

## Design Decisions

- **NoSQL Database:**  
  MongoDB Atlas is used for its flexible schema, reducing the number of collections needed and allowing dynamic data modeling.

- **Security:**  
  User authentication and authorization are handled with flask-login and password protection methods to ensure secure access.

## User Guide

- **Home Page:**  
  Displays a list of available products. Users can:
  - Search by product name,
  - Filter by category (e.g., Antique Furniture, GPS Watches, Running Shoes, Vinyls),
  - Sort products by price or rating.

- **Product Details:**  
  Clicking on a product opens its detail page, which displays:
  - Product image, description, seller, category-specific fields (e.g., material, size, battery life),
  - User reviews and average rating,
  - Related products from the same category.  
  Logged-in users can:
  - Submit or update their rating (1–10),
  - Write or edit a review.

- **Login and Register Pages:**  
  - New users can create an account with a username and password.
  - Existing users can log in to access protected features like rating, reviewing, and viewing their profile.

- **User Profile:**  
  Accessible only to authenticated users. Displays:
  - User’s average rating across all reviewed items,
  - A list of all written reviews,
  - Dates and item names for each rating and review.

- **Admin Dashboard:**  
  Accessible only to admin users. Admins can:
  - View a full list of users and items,
  - Navigate to item or user management pages,
  - Remove any existing user or product.

- **Add Item Page:**  
  Admins can add new products by filling out a form that includes:
  - Name, description, price, seller, image link,
  - Optional fields like age, battery life, size, and material,
  - Category selection from predefined categories.

- **Add User Page:**  
  Admins can create new users by specifying:
  - Username, password, and user role (`user` or `admin`).


## Login Instructions

### Regular User:
- **Registration:** Create a new account via the registration page.
- **Login:** Use your username and password on the login page to access the application.

### Admin User:
- An admin account can be pre-defined or created by promoting a regular user.
- After logging in, admin users can access the admin dashboard through the **Admin** link in the navigation bar.

