


https://github.com/shivamkumarsingh28/Go_svelte_Project/assets/110661272/ab98839e-7c32-44fd-9df2-76c3452588db


Assignment: E-commerce Platform Development
Overview:
Develop a simplified e-commerce platform where users can browse products, add them to a cart, and proceed to checkout. The platform should feature product management, user authentication, cart functionality, and order processing.
Backend (Golang):
API Design:

Design RESTful APIs to handle CRUD operations for products, users, carts, and orders.
Implement authentication and authorization. Use JWT for managing user sessions.
Ensure all API responses are returned in a consistent and RESTful manner.
Database Integration:

Choose an appropriate SQL or NoSQL database to store user data, product information, cart data, and orders.
Design the database schema and implement migrations.
Business Logic:

Product Management: Include functionality to add, update, delete, and list products. Products should have fields like name, description, price, and stock quantity.
Cart Management: Implement logic to add items to a cart, update item quantity, remove items, and clear the cart.
Order Processing: Create a workflow for converting a cart into an order. Include basic order management like viewing past orders.
Security:

Implement secure endpoints. Ensure that passwords are hashed before storage.
Validate all incoming data to prevent SQL injection and other common security threats.
Bonus Challenges:

Integrate a third-party payment gateway (e.g., Stripe, PayPal) for processing payments.
Implement simple product search and filtering capabilities.
Frontend (Svelte):
User Interface:

Create a clean and responsive design for the platform.
Implement pages for product listing, product details, user registration/login, cart, and checkout process.
State Management:

Manage application state effectively, handling user sessions, cart data, and alert messages (e.g., for errors or confirmations).
API Integration:

Integrate the frontend with the backend APIs. Display products, manage user authentication, handle cart operations, and submit orders.
Dynamic Interactions:

Ensure the product listings and cart contents update dynamically as users interact with the platform.
Implement form validations for user input (e.g., during registration, login, and checkout).
Bonus Challenges:

Add client-side routing to create a single-page application (SPA) experience.
Implement progressive web app (PWA) features for offline capabilities and a mobile-friendly experience.
Deliverables:
Source code for both the backend and frontend, including any database schema migrations and seed data for testing.
Documentation covering:
API endpoints and their usage.
Instructions for setting up the development environment, running the application, and deploying it.
Any assumptions made and decisions taken during development.
Evaluation Criteria:
Functionality: The application should meet all the basic requirements, with bonus features considered for extra credit.
Code Quality: The code should be clean, well-organized, and properly commented.
Design and UX: The frontend should be user-friendly, with intuitive navigation and a responsive design.
Security and Best Practices: The application should follow security best practices, especially in handling user data and interactions with the backend.
Documentation: The provided documentation should be clear and comprehensive, enabling easy setup and understanding of the application.
This assignment is designed to mimic the challenges faced in real-world full-stack development, providing a holistic view of the candidate's technical skills, problem-solving abilities, and attention to detail.
