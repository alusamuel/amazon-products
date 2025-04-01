# Premium Product Search On Amazon

## Overview
This project is a responsive, visually appealing web application designed to showcase premium products in an e-commerce-like interface. The application includes advanced features such as product filtering for detailed product views, and interactive elements like toast notifications. The design leverages modern CSS techniques and JavaScript to create a seamless user experience.

The application fetches product data from an external API (currently using a demo API endpoint) and dynamically renders the products in a grid layout. Users can interact with the products through searching.

## Technologies Used

### Backend Server
- **Node.js**: Backend runtime environment
- **Express.js**: Web framework for handling API requests
- **PM2**: Process manager for Node.js applications, ensuring uptime and reliability
- **Nginx**: Reverse proxy server for handling HTTP requests and load balancing
- **RapidAPI**: Used to integrate third-party APIs into the backend

### Frontend Server
- **HTML, CSS, JavaScript**: Used for building the frontend interface
- **Nginx**: Serves the frontend application efficiently

## Key Features

1. **Responsive Design**:
   - Fully responsive layout optimized for both desktop and mobile devices.
   - Uses CSS Grid and Flexbox for flexible layouts.

2. **Dynamic Content Loading**:
   - Fetches product data from an external API (e.g., Amazon Data API).
   - Displays a loading spinner while data is being fetched.

3. **Interactive Product Cards**:
   - Each product card includes hover effects, quick action buttons (favorite, share, compare), and detailed metadata (price, rating, availability).

7. **Filter and Sort Options**:
   - Includes UI elements for filtering and sorting products (functionality can be extended further).

8. **Error Handling**:
   - Displays error messages if the API request fails or no products are found.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/alusamuel/amazon-products.git
   cd amazon-products
   ```

2. Install dependencies for the backend:
   ```bash
   cd backend
   npm install express node-fetch cors
   ```

3. Start the backend server using PM2:
   ```bash
   pm2 start server.js --name backend
   ```

4. Set up Nginx as a reverse proxy for the backend.

5. Open `index.html` in a browser to view the frontend.

## Deployment
Ensure that both the frontend and backend servers are correctly configured with Nginx, and PM2 is managing the backend processes efficiently.

## Future Enhancements

1. **Backend Integration**:
   - Implement a backend service to handle cart management and user authentication.

2. **Advanced Filtering and Sorting**:
   - Add more robust filtering options (e.g., by category, price range).

3. **Performance Optimization**:
   - Implement lazy loading for images and infinite scrolling for large datasets.

4. **Accessibility Improvements**:
   - Ensure full compliance with WCAG guidelines for accessibility.

## Video Demonstration

[Insert video link here]

## Contribution
Feel free to fork the repository and submit pull requests with improvements.

