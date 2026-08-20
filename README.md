# Pharmacy Management System

An online pharmacy web application with an e-commerce storefront for medicines and a telemedicine module for booking doctor appointments.

## Features

- User authentication with email based login and role selection (Patient or Doctor) at signup
- Product catalog with categories, product listing, and product detail pages
- Shopping cart with add, remove, and delete functionality
- Checkout flow with tax and total calculation
- Doctor listing with specialization and availability
- Appointment booking with prescription file upload and status tracking (Pending, Confirmed, Cancelled)
- Admin panel for managing users, products, categories, carts, doctors, and appointments

## Tech Stack

- **Backend:** Python, Django
- **Database:** SQLite, Django ORM
- **Frontend:** HTML, CSS, Bootstrap 4, jQuery
- **Architecture:** Django MVT (Model View Template)

## Architecture

The project is a single Django application split into five apps, each handling one domain:

- **accounts** – custom user model and authentication
- **category** – product categories
- **store** – product catalog
- **carts** – cart and checkout
- **doctor** – doctor profiles and appointments

Each app has its own models, views, urls, and admin configuration, connected through a single root URL configuration and a shared set of templates.
