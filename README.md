React E-Commerce Application

Live Demo: am-react-ecommerce.netlify.app
This is a professional-grade, full-stack React application designed to demonstrate modern web development patterns. It features a robust product system, persistent authentication, and global state management.
🚀 Quick Start
Get your development environment up and running in seconds using Vite.
bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
Use code with caution.

🛠️ Core Architecture
1. State Management (Context API)
The application utilizes the React Context API to manage global states without "prop drilling."
AuthContext: Handles user sessions and persistence via localStorage.
CartContext: Manages shopping cart logic, including immutable state updates for adding, removing, and calculating totals.

2. Custom Hooks
To keep components clean and reusable, logic is abstracted into Custom Hooks:
useAuth(): Simplifies access to user data and login/logout methods.
useCart(): Provides a streamlined interface for interacting with the shopping basket.

3. Routing & Navigation
Powered by React Router, the app features:
Dynamic Routes: products/:id for detailed product views.
Programmatic Navigation: Redirects users post-authentication using useNavigate.
Protected UI: Conditional rendering based on authentication state.

📦 Key Features
Authentication System
Persistence: Sessions survive page refreshes using localStorage.
Security: Implements generic error handling to prevent credential enumeration.
Shopping Experience
Dynamic Catalog: Renders products via .map() with unique keys for performance.
Logic-Heavy Cart:
Prevents duplicate entries.
Uses .reduce() for real-time total price calculation.
Uses .filter() and .map() for immutable quantity adjustments.
Data Synchronization
Side Effects: Uses useEffect to synchronize the UI with URL parameters and fetch data.
UX Design: Built-in loading states and null-checks to prevent application crashes during data fetching.

🌐 Deployment
This project is deployed and hosted on Netlify. Every push to the main branch triggers an automated CI/CD pipeline for instant updates.