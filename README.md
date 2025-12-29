🛍️ E-Commerce Platform



A production-ready, single-store e-commerce system combining the simplicity of YouCan with the power of Shopify.








🎯 Overview

A complete, modern e-commerce platform built with:





Backend: Node.js + Express + PostgreSQL



Frontend: React + Vite + Tailwind CSS



Architecture: REST API with JWT authentication



Design: Mobile-first, responsive, and user-friendly

Perfect for entrepreneurs, small businesses, and developers who want to launch an online store quickly.



✨ Key Features

🏪 Store Features





✅ Responsive homepage with hero section



✅ Product catalog with categories



✅ Advanced filtering (price, category, search)



✅ Product details with image gallery



✅ Shopping cart (persistent, AJAX)



✅ Checkout with form validation



✅ Cash on Delivery (COD) payment



✅ Order confirmation page



✅ WhatsApp order notifications



✅ SEO-friendly URLs



✅ Mobile-first responsive design

👨‍💼 Admin Dashboard





✅ Secure admin login with JWT



✅ Dashboard overview with KPIs



✅ Product management (CRUD)



✅ Product variants (size, color)



✅ Multiple product images



✅ Duplicate product feature



✅ Order management with status tracking



✅ Customer management



✅ Discount code management



✅ Shipping settings by city



✅ Inventory management



✅ Analytics and reports



✅ Email notifications



✅ CSV export functionality

🚀 Advanced Features





✅ Inventory auto-decrease on order



✅ Out-of-stock protection



✅ Discount codes (percentage/fixed)



✅ Email order confirmations



✅ WhatsApp integration



✅ Analytics dashboard



✅ Draft products



✅ SEO meta tags



✅ Low stock alerts



✅ Order history per customer



📋 Tech Stack

Backend





Runtime: Node.js 18+



Framework: Express.js



Database: PostgreSQL



ORM: Sequelize



Authentication: JWT



Password Hashing: bcryptjs



Validation: Joi



Email: Nodemailer

Frontend





Library: React 18+



Build Tool: Vite



Styling: Tailwind CSS



HTTP Client: Axios



Routing: React Router v6



State Management: Context API



Forms: React Hook Form



🚀 Quick Start

Prerequisites





Node.js 18+



PostgreSQL 12+



npm 9+

Installation

# 1. Clone repository
git clone https://github.com/yourusername/ecommerce-platform.git
cd ecommerce-platform

# 2. Setup Database
createdb ecommerce_db
psql -U postgres -d ecommerce_db -f DATABASE_SCHEMA.sql

# 3. Setup Backend
cd backend
cp .env.example .env
# Edit .env with your settings
npm install
npm run dev

# 4. Setup Frontend (in new terminal)
cd frontend
cp .env.example .env
npm install
npm run dev


Access the Application





Store: http://localhost:5173



Admin Dashboard: http://localhost:5173/admin



API: http://localhost:5000/api

Default Admin Credentials





Email: admin@example.com



Password: Admin@123456

⚠️ Change these immediately in production!



📁 Project Structure

ecommerce-platform/
├── backend/
│   ├── config/              # Configuration files
│   ├── models/              # Database models
│   ├── controllers/         # Request handlers
│   ├── services/            # Business logic
│   ├── routes/              # API routes
│   ├── middleware/          # Custom middleware
│   ├── utils/               # Utility functions
│   ├── server.js            # Express app
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── pages/           # Page components
│   │   ├── hooks/           # Custom hooks
│   │   ├── context/         # Context providers
│   │   ├── services/        # API services
│   │   ├── styles/          # CSS files
│   │   ├── utils/           # Utility functions
│   │   └── App.jsx
│   ├── public/              # Static assets
│   └── package.json
│
├── docs/                    # Documentation
├── DATABASE_SCHEMA.sql      # Database schema
├── API_ENDPOINTS.md         # API documentation
├── SETUP_GUIDE.md          # Setup instructions
└── README.md




📚 Documentation





Setup Guide - Complete installation and setup instructions



API Documentation - All API endpoints with examples



Project Documentation - Architecture and design



Database Schema - Database structure



🔐 Security Features





✅ JWT authentication



✅ Password hashing with bcryptjs



✅ CORS protection



✅ Rate limiting



✅ Input validation



✅ SQL injection prevention (Sequelize ORM)



✅ XSS protection (React)



✅ Helmet.js security headers



📊 API Overview

Authentication

POST   /api/auth/login              - Admin login
POST   /api/auth/logout             - Admin logout
POST   /api/auth/refresh-token      - Refresh JWT token
GET    /api/auth/me                 - Get current user


Products

GET    /api/products                - List all products
GET    /api/products/:id            - Get product details
POST   /api/admin/products          - Create product (admin)
PUT    /api/admin/products/:id      - Update product (admin)
DELETE /api/admin/products/:id      - Delete product (admin)


Orders

POST   /api/orders                  - Create order
GET    /api/orders/:id              - Get order details
GET    /api/admin/orders            - List all orders (admin)
PUT    /api/admin/orders/:id/status - Update order status (admin)


More endpoints available in API_ENDPOINTS.md



🧪 Testing

Manual Testing





Test Store Flow





Browse products



Add to cart



Checkout



Place order



Test Admin Functions





Login to admin



Create/edit products



Manage orders



View analytics

API Testing

# Using cURL
curl http://localhost:5000/api/products

# Using Postman
# Import API collection (coming soon)




🚀 Deployment

Backend Deployment Options





Heroku



Railway



Render



AWS EC2



DigitalOcean

Frontend Deployment Options





Vercel



Netlify



AWS S3 + CloudFront



GitHub Pages

Production Checklist





Update environment variables



Set secure JWT secret



Configure email service



Enable HTTPS



Configure CORS properly



Set up database backups



Configure CDN for images



Set up monitoring and logging



Test all payment flows



🔄 Development Workflow

# Terminal 1: Backend
cd backend
npm run dev

# Terminal 2: Frontend
cd frontend
npm run dev

# Terminal 3: Database (if needed)
psql -U postgres -d ecommerce_db




📦 Available Scripts

Backend

npm run dev          # Start development server
npm start            # Start production server
npm run migrate      # Run database migrations
npm run seed         # Seed database with sample data
npm test             # Run tests
npm run lint         # Run ESLint


Frontend

npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run lint         # Run ESLint




🐛 Troubleshooting

Common Issues

Database Connection Error

# Ensure PostgreSQL is running
brew services start postgresql  # macOS
sudo systemctl start postgresql # Linux


Port Already in Use

# Change PORT in .env or kill process
lsof -i :5000
kill -9 <PID>


Dependencies Not Installed

# Reinstall dependencies
rm -rf node_modules package-lock.json
npm install


See SETUP_GUIDE.md for more troubleshooting tips.



🎨 Customization

Branding





Update store name in .env



Replace logo in frontend/public/



Customize colors in tailwind.config.js

Features





Add payment gateways (Stripe, PayPal)



Implement email marketing



Add product reviews



Create wishlist functionality

Integrations





WhatsApp Business API



Email service (SendGrid, Mailgun)



SMS notifications



Analytics (Google Analytics, Mixpanel)



📈 Future Enhancements





Payment gateway integration (Stripe, PayPal)



Product reviews and ratings



Wishlist functionality



Email marketing integration



SMS notifications



Multi-language support



Multi-currency support



Advanced analytics



Inventory forecasting



Automated email campaigns



📞 Support

For issues, questions, or suggestions:





Check the documentation



Review API endpoints



Check setup guide



Open an issue on GitHub



📄 License

This project is licensed under the MIT License - see the LICENSE file for details.



👨‍💻 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.





Fork the repository



Create your feature branch (git checkout -b feature/AmazingFeature)



Commit your changes (git commit -m 'Add some AmazingFeature')



Push to the branch (git push origin feature/AmazingFeature)



Open a Pull Request



🙏 Acknowledgments





Inspired by YouCan's simplicity



Powered by Shopify's features



Built with modern web technologies



📊 Project Stats





Lines of Code: 5000+



Database Tables: 12



API Endpoints: 40+



React Components: 30+



Setup Time: ~30 minutes



🎯 Roadmap

Phase 1 (Current)





✅ Core e-commerce functionality



✅ Admin dashboard



✅ Product management



✅ Order management

Phase 2





Payment gateway integration



Advanced analytics



Email marketing



SMS notifications

Phase 3





Mobile app



Multi-vendor support



Subscription products



Advanced inventory management



Made with ❤️ for entrepreneurs and developers

Last Updated: December 2024
Version: 1.0.0
Status: Production Ready
