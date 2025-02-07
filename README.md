# Food Site

A modern React-based e-commerce platform for Food, featuring a shopping cart system and responsive design.

## Features

- Product catalog with categories
- Interactive shopping cart with add/remove functionality
- Product filtering and search
- Responsive design for mobile and desktop
- User authentication system
- Cart persistence using localStorage

## Components Structure

### Main Components
- `Header` - Navigation and cart summary
- `ProductList` - Displays all available snacks
- `ProductCard` - Individual snack display component
- `Cart` - Shopping cart management
- `FilterSection` - Product filtering options
- `SearchBar` - Product search functionality

### Data Structure
```javascript
// Product Structure
const productShape = {
  id: Number,
  name: String,
  price: Number,
  image: String,
  category: String,
  description: String
};

// Cart Item Structure
const cartItemShape = {
  product: productShape,
  quantity: Number
};
```

## Technologies Used

- React.js
- JavaScript
- CSS/SCSS
- Node.js

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/thulasidharan96/Food-Site.git
```

2. Navigate to the project directory:
```bash
cd Food-Site
```

3. Install dependencies:
```bash
npm install
```

4. Start the development server:
```bash
npm start
```

The application will open in your default browser at `http://localhost:3000`

### Environment Variables
```
REACT_APP_API_URL=your_api_url
REACT_APP_STORAGE_KEY=your_storage_key
```

## Available Scripts

- `npm start` - Runs the app in development mode
- `npm test` - Launches the test runner
- `npm run build` - Builds the app for production
- `npm run eject` - Ejects from Create React App


## State Management

The application uses React Context API for global state management:
- CartContext for shopping cart state
- Custom hooks for cart and product management
- localStorage for cart persistence

## API Integration

The application interacts with a REST API with the following endpoints:
- GET `/products` - Fetch all products
- GET `/products/:id` - Fetch single product
- GET `/categories` - Fetch product categories

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.