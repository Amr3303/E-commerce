# E-commerce Backend API

A robust Node.js backend API for an E-commerce application with features like user management, product catalog, shopping cart, and coupon system.

## Features

- User Authentication & Authorization
- Product Management
- Category Management
- Shopping Cart Functionality
- Coupon System
- File Upload Support
- Email Notifications
- MongoDB Database Integration

## Tech Stack

- Node.js
- Express.js
- MongoDB
- JWT Authentication
- Multer for file uploads
- Nodemailer for email notifications

## Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

## Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd E-commerce-app
```

2. Install dependencies:

```bash
npm install
```

3. Create a `.env` file in the root directory with the following variables:

```env
MONGODB_URI=your_mongodb_connection_string
PORT=5000
```

4. Start the server:

```bash
npm start
```

## API Endpoints

### Users

- POST `/api/users/register` - Register a new user
- POST `/api/users/login` - User login
- GET `/api/users/profile` - Get user profile
- PUT `/api/users/profile` - Update user profile

### Products

- GET `/api/products` - Get all products
- GET `/api/products/:id` - Get product by ID
- POST `/api/products` - Create new product
- PUT `/api/products/:id` - Update product
- DELETE `/api/products/:id` - Delete product

### Categories

- GET `/api/categories` - Get all categories
- POST `/api/categories` - Create new category
- PUT `/api/categories/:id` - Update category
- DELETE `/api/categories/:id` - Delete category

### Cart

- GET `/api/cart` - Get user's cart
- POST `/api/cart` - Add item to cart
- PUT `/api/cart/:id` - Update cart item
- DELETE `/api/cart/:id` - Remove item from cart

### Coupons

- GET `/api/coupons` - Get all coupons
- POST `/api/coupons` - Create new coupon
- PUT `/api/coupons/:id` - Update coupon
- DELETE `/api/coupons/:id` - Delete coupon

## File Upload

The application supports file uploads for product images. Uploaded files are stored in the `uploads` directory and are served statically.

## Error Handling

The API implements comprehensive error handling for:

- Validation errors
- Authentication errors
- Database errors
- File upload errors

## Security Features

- JWT-based authentication
- Password hashing with bcrypt
- Input validation using Joi
- CORS enabled
- Secure file upload handling

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request