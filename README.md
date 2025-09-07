# Real-Time Inventory and Product Management System

## Overview
A comprehensive web-based system for managing inventory, production, orders, and delivery operations for a food production business specializing in milk and tofu products.

## Features
- Multi-user role-based access control
- Real-time inventory tracking
- Production management
- Order processing and billing
- Customer relationship management
- Delivery tracking system
- Analytics and reporting

## Tech Stack
- **Backend**: Python Flask
- **Database**: SQLite with SQLAlchemy ORM
- **Frontend**: HTML, CSS, JavaScript
- **UI Components**: Dash, Plotly
- **Visualization**: Bokeh

## Installation

### Prerequisites
- Python 3.10 or higher
- pip package manager
- Git

### Setup Steps

1. **Clone the repository**
```bash
git clone <repository-url>
cd RealTime-Inventory-And-Product-management-System
```

2. **Create and activate virtual environment**
```bash
python -m venv myenv
myenv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Initialize the database**
```bash
python database.py
```

5. **Start the application**
```bash
python app.py
```

The application will be available at `http://localhost:5000`

## Default Users

| Username | Password | Role |
|----------|----------|------|
| admin | admin | Administrator |
| john_doe | password1 | Production Manager |
| jane_smith | password2 | Delivery Person |

## Project Structure

### Core Components
- `/templates` - HTML templates for all pages
- `/static` - Static assets (CSS, JS, images)
- `/instance` - Database files
- `app.py` - Main application file
- `database.py` - Database initialization

### Key Features by Role

#### Administrator
- User management
- System-wide access
- Analytics dashboard
- Inventory overview

#### Production Manager
- Manage raw materials
- Track production
- Update inventory
- Manage products

#### Order Manager
- Process orders
- Customer management
- Generate bills
- Track deliveries

#### Delivery Person
- View assigned deliveries
- Update delivery status
- Manage route information

## Database Schema

### Core Tables
- Users
- Inventory (Milk, Tofu, General)
- Products
- Orders
- Customers
- DeliveryPerson
- Production

## API Endpoints

### Authentication
- `/login` - User login
- `/logout` - User logout
- `/register` - New user registration

### Inventory Management
- `/inventory` - View inventory
- `/add_inventory` - Add new inventory
- `/update_inventory` - Update existing inventory

### Order Management
- `/orders` - View orders
- `/add_order` - Create new order
- `/update_order` - Update order status

### Production Management
- `/production` - View production
- `/add_production` - Add production record
- `/update_production` - Update production details

## Security Features
- Session-based authentication
- Role-based access control
- Password hashing
- Protected routes

## Development

### Running in Debug Mode
```bash
python app.py --debug
```

### Database Management
```bash
# Reset database
python database.py --reset
```

## Contributing
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License
MIT License

## Support
For support and queries, please create an issue in the repository.

## Authors
[PythonIndian](https://github.com/PythonIndian)

---

**Note**: This system is designed for production environments. Ensure proper security measures are implemented before deployment.

For more detailed documentation, refer to the individual module documentation in the source code.