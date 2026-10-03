# Architecture

Vanilla Shop follows a modular Django architecture designed for an e-commerce application.

## Project Structure

```text
vanilla/
├── account/      # Authentication, users, profiles and addresses
├── product/      # Products, variants, reviews and categories
├── cart/         # Shopping cart and cart items
├── order/        # Orders, payments, discounts and returns
├── wishlist/     # User wishlists
├── blog/         # Blog and content management
├── home/         # Homepage and site settings
└── vanilla/      # Project configuration, URLs and WSGI
```

## Main Flow

```text
User
 ↓
Django Views / REST API
 ↓
Business Logic & Services
 ↓
Django Models
 ↓
PostgreSQL
```

The project separates major business areas into independent Django apps, making the codebase easier to maintain and extend.

## Authentication

User authentication is based on phone-number verification and OTP. JWT is used for API authentication.

## Frontend

The storefront uses HTML, CSS and JavaScript with a responsive layout for desktop and mobile devices.

## Deployment

The application is deployed with Python, Django and Passenger on a cPanel-based hosting environment.
