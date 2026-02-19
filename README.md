React E-Commerce Application

Live Demo: https://am-react-ecommerce.netlify.app

📌 Project Overview

This project is a full-stack, production-ready React E-Commerce application built to demonstrate modern frontend architecture and scalable state management patterns.

The application simulates a real-world online shopping platform, featuring product browsing, authentication, cart management, protected routes, and persistent user sessions. It is designed with clean code principles, reusable logic, and performance optimization in mind.

⚙️ Tech Stack

Frontend: React (Vite)

State Management: React Context API

Routing: React Router

Authentication: Local Storage-based session persistence

Deployment: Netlify (CI/CD enabled)

🚀 Getting Started
1️⃣ Install Dependencies
npm install

2️⃣ Run Development Server
npm run dev

3️⃣ Build for Production
npm run build

🏗️ Application Architecture
1. Global State Management

The application uses the React Context API to manage shared state across components without prop drilling.

🔐 AuthContext

Handles login/logout functionality

Persists user session using localStorage

Provides authentication state globally

Prevents unauthorized access to protected routes

🛒 CartContext

Manages shopping cart state

Prevents duplicate product entries

Supports quantity updates using immutable patterns

Calculates totals dynamically using .reduce()

2. Custom Hooks

Business logic is abstracted into reusable hooks to maintain clean component structure:

useAuth() – Access authentication state and methods

useCart() – Interact with cart state and cart actions

This improves scalability and separation of concerns.

3. Routing & Navigation

Powered by React Router:

Dynamic Routing: /products/:id

Programmatic Navigation: Redirect after authentication using useNavigate

Protected UI: Conditional rendering based on authentication state

🛍️ Core Features
✅ Authentication System

Session persistence across page refresh

Secure login handling with generic error messaging

Protected pages for authenticated users

✅ Product Catalog

Dynamic product rendering using .map()

Unique keys for optimized rendering

Real-time product detail view

✅ Shopping Cart Logic

Prevents duplicate cart entries

Immutable updates using .map() and .filter()

Real-time total calculation using .reduce()

Automatic UI updates via Context state

✅ Data Handling & UX

useEffect for side-effect management

Loading states during data fetching

Defensive null-checks to prevent crashes

Clean and responsive user interface

🌍 Deployment & CI/CD

The application is deployed on Netlify.

Automatic deployment on every push to the main branch

Continuous Integration & Continuous Deployment (CI/CD)

Production build optimization via Vite

🎯 Purpose of the Project

This project was developed to:

Demonstrate advanced React patterns

Showcase scalable state management

Apply real-world authentication handling

Practice clean architecture and reusable logic

Simulate an actual e-commerce workflow