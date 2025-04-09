# Product Store

A full-stack web application for managing product inventory with CRUD operations. Built with React, Express, MongoDB, and Chakra UI.

![Product Store Screenshot](https://placehold.co/600x400?text=Product+Store+App)

## Features

- **View Products**: Browse all products in a responsive grid layout
- **Create Products**: Add new products with name, price, and image URL
- **Update Products**: Edit existing product details
- **Delete Products**: Remove products from the inventory
- **Responsive Design**: Works on mobile, tablet, and desktop views

## Tech Stack

### Frontend

- **React** with Vite for fast development
- **Chakra UI** for a modern, accessible component library
- **React Router** for page navigation
- **Zustand** for global state management

### Backend

- **Express.js** for the API server
- **MongoDB** with Mongoose for data storage
- **RESTful API** architecture

## API Endpoints

| Method | Endpoint          | Description            |
| ------ | ----------------- | ---------------------- |
| GET    | /api/products     | Retrieve all products  |
| POST   | /api/products     | Create a new product   |
| PUT    | /api/products/:id | Update a product by ID |
| DELETE | /api/products/:id | Delete a product by ID |

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (local or Atlas connection)

### Installation

1. Clone the repository

   ```bash
   git clone https://github.com/devSayan619/PRODUCT-STORE.git
   cd product-store
   ```

2. Set up the backend

   ```bash
   cd backend
   npm install
   ```

3. Create a `.env` file in the backend directory with the following:

   ```
   MONGO_URI=your_mongodb_connection_string
   PORT=6969
   ```

4. Set up the frontend

   ```bash
   cd ../frontend
   npm install
   ```

5. Run the application

   In the backend directory:

   ```bash
   npm run dev
   ```

   In the frontend directory:

   ```bash
   npm run dev
   ```

6. Open your browser and go to `http://localhost:5173`

## Project Structure

```
product-store/
├── backend/
│   ├── config/
│   │   └── db.js
│   ├── controllers/
│   │   └── product.controller.js
│   ├── models/
│   │   └── product.model.js
│   ├── routes/
│   │   └── product.route.js
│   └── server.js
└── frontend/
    ├── public/
    ├── src/
    │   ├── components/
    │   │   ├── Navbar.jsx
    │   │   └── ProductCard.jsx
    │   ├── pages/
    │   │   ├── CreatePage.jsx
    │   │   └── HomePage.jsx
    │   ├── store/
    │   │   └── product.js
    │   ├── App.jsx
    │   └── main.jsx
    ├── index.html
    └── vite.config.js
```

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Chakra UI for the component library
- Zustand for lightweight state management
- MongoDB for database services
