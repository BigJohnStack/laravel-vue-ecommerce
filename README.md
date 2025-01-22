# E-Commerce Platform (Laravel + Vue.js)

Welcome to the **E-Commerce Platform**, a powerful and customizable e-commerce solution built with **Laravel** for the backend and **Vue.js** for the frontend. This application is designed to provide a seamless shopping experience with a modern and responsive user interface.

---

## Features

- **User Authentication & Role Management**  
  Secure login, registration, and admin-user roles.

- **Product Management**  
  Add, edit, and manage products with categories, pricing, and inventory.

- **Shopping Cart**  
  Dynamic shopping cart with real-time updates.

- **Order Management**  
  Customers can place orders, and admins can manage order statuses.

- **Payment Integration**  
  Integrated with popular payment gateways (e.g., PayPal, Stripe).

- **Responsive Design**  
  Optimized for desktop and mobile devices.

- **Admin Dashboard**  
  Manage users, products, and orders with a feature-rich admin panel.

---

## Requirements

### Backend
- PHP 8.1 or higher
- Laravel 10
- MySQL 8.0 or PostgreSQL 13+
- Composer

### Frontend
- Node.js 18+ (with npm or Yarn)
- Vue CLI

### Others
- Redis (for caching and queues)
- Web server (Apache/Nginx)

---

## Installation

### Backend (Laravel)
1. Clone the repository:  
   ```bash
   git clone https://github.com/bigjohnstack/ecommerce-backend.git
   cd ecommerce-backend
   ```

2. Install dependencies:  
   ```bash
   composer install
   ```

3. Configure environment variables:  
   Copy the `.env.example` to `.env` and set the database, mail, and storage configurations.  
   ```bash
   cp .env.example .env
   ```

4. Generate application key:  
   ```bash
   php artisan key:generate
   ```

5. Run migrations and seeders:  
   ```bash
   php artisan migrate --seed
   ```

6. Start the server:  
   ```bash
   php artisan serve
   ```

### Frontend (Vue.js)
1. Navigate to the frontend directory:  
   ```bash
   cd ecommerce-frontend
   ```

2. Install dependencies:  
   ```bash
   npm install
   ```

3. Configure environment:  
   Edit the `src/config.js` file to point to your backend API.

4. Build and serve the application:  
   ```bash
   npm run serve
   ```

---

## Usage

1. Access the application at:  
   - Backend: `http://localhost:8000`  
   - Frontend: `http://localhost:8080`

2. Login with the default admin credentials (from seeders):  
   - **Email**: `admin@bigjohnstack.com`  
   - **Password**: `password`

3. Start managing products and enjoy the shopping experience!

---

## API Documentation

The backend provides a RESTful API for communication with the frontend. You can find the API documentation via **Postman Collection** or by visiting `http://localhost:8000/api/documentation`.

---

## Testing

### Backend
Run Laravel tests:  
```bash
php artisan test
```

### Frontend
Run Vue.js tests:  
```bash
npm run test
```

---

## Deployment

### Backend
1. Set up a production server with PHP, MySQL/PostgreSQL, and Composer.
2. Use a web server (e.g., Nginx) to serve the Laravel application.
3. Configure `.env` for production and run migrations:  
   ```bash
   php artisan migrate --force
   ```

### Frontend
1. Build the Vue.js app for production:  
   ```bash
   npm run build
   ```
2. Deploy the `dist` folder to a static file server or a cloud provider (e.g., AWS S3, Firebase).

---

## Contributing

1. Fork the repository.
2. Create a new branch:  
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:  
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to the branch:  
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Support

For issues or questions, please open an issue on [GitHub](https://github.com/bigjohnstack/ecommerce) or contact **bigjohnstack.dev@gmail.com**.
