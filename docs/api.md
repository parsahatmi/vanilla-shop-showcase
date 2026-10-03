# API Overview

Vanilla Shop provides a REST API powered by Django REST Framework.

## API Areas

The API is organized around the main business domains of the application:

```text
Authentication
Products
Cart
Wishlist
Orders
Payments
Profile & Addresses
Blog
```

## Authentication

Authenticated requests use JWT tokens.

Typical authentication flow:

```text
Phone Number
    ↓
OTP Verification
    ↓
JWT Authentication
    ↓
Authenticated API Requests
```

## API Design

The API follows standard HTTP methods where appropriate:

```text
GET     → Retrieve data
POST    → Create data
PUT/PATCH → Update data
DELETE  → Remove data
```

Detailed endpoint documentation can be added as the API evolves.
