# RENART - Luxury Jewelry E-commerce Platform

## Overview

RENART is a comprehensive luxury jewelry e-commerce platform consisting of three interconnected applications that provide a complete solution for online jewelry retail. The platform combines modern web technologies with elegant design to deliver an exceptional user experience for both customers and vendors.

## Project Architecture

This repository serves as an umbrella project containing three core components:

### 🛍️ Online Store (`online-store/`)
- **Repository**: [renart-online-store](https://github.com/bedirhantong/renart-online-store.git)
- **Technology**: Next.js 14, TypeScript, Tailwind CSS
- **Purpose**: Customer-facing e-commerce application
- **Features**:
  - Product catalog with advanced filtering
  - Interactive product galleries with zoom and carousel
  - User authentication and favorites system
  - Responsive design with luxury aesthetics
  - Shopping cart and checkout flow
  - Modern animations and transitions

### 🖥️ Backend API (`backend/`)
- **Repository**: [RENART-Backend](https://github.com/bedirhantong/RENART-Backend.git)
- **Technology**: Node.js, Express, MongoDB
- **Purpose**: RESTful API serving both frontend applications
- **Features**:
  - Product management and inventory
  - User authentication and authorization
  - Order processing and tracking
  - Vendor management system
  - Secure API endpoints with validation
  - Database optimization and indexing

### 📊 Vendor Panel (`vendor-panel/`)
- **Repository**: [renart-vendor-panel](https://github.com/bedirhantong/renart-vendor-panel.git)
- **Technology**: React, TypeScript, Material-UI
- **Purpose**: Vendor dashboard for product and order management
- **Features**:
  - Product catalog management
  - Order tracking and fulfillment
  - Analytics and reporting
  - Inventory management
  - Vendor profile management

## Getting Started

### Prerequisites

Ensure you have the following installed:
- **Node.js** (v18 or higher)
- **npm** or **yarn**
- **MongoDB** (local or cloud instance)
- **Git**

### Clone the Repository

```bash
# Clone the umbrella repository with all submodules
git clone --recursive https://github.com/bedirhantong/RENART-Full-Project.git

# Or if already cloned, initialize submodules
git submodule update --init --recursive
```

### Setup Instructions

1. **Backend Setup**
   ```bash
   cd backend
   npm install
   cp .env.example .env
   # Configure your environment variables
   npm run dev
   ```

2. **Online Store Setup**
   ```bash
   cd online-store
   npm install
   cp .env.local.example .env.local
   # Configure your environment variables
   npm run dev
   ```

3. **Vendor Panel Setup**
   ```bash
   cd vendor-panel
   npm install
   cp .env.example .env
   # Configure your environment variables
   npm start
   ```

## Development Workflow

### Working with Submodules

When making changes to individual components:

```bash
# Navigate to specific submodule
cd online-store/

# Make your changes and commit
git add .
git commit -m "feat: add new feature"
git push origin main

# Return to umbrella repo and update submodule reference
cd ..
git add online-store
git commit -m "update: online-store submodule"
git push origin main
```

### Updating All Submodules

```bash
# Pull latest changes for all submodules
git submodule update --recursive --remote

# Commit the updated references
git add .
git commit -m "update: all submodules to latest"
git push origin main
```

## Technology Stack

### Frontend Technologies
- **Next.js 14** - React framework with SSR/SSG capabilities
- **TypeScript** - Type-safe JavaScript development
- **Tailwind CSS** - Utility-first CSS framework
- **React Query** - Data fetching and caching
- **Framer Motion** - Animation library

### Backend Technologies
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **JWT** - Authentication and authorization
- **Multer** - File upload handling

### DevOps & Tools
- **ESLint** - Code linting
- **Prettier** - Code formatting
- **Husky** - Git hooks
- **Docker** - Containerization (optional)

## Key Features

### 🎨 Modern Design
- Luxury jewelry store aesthetics
- Responsive design across all devices
- Smooth animations and micro-interactions
- Professional color scheme and typography

### 🔐 Security
- JWT-based authentication
- Input validation and sanitization
- Secure API endpoints
- Environment-based configuration

### 📱 User Experience
- Intuitive navigation and search
- Advanced product filtering
- Interactive product galleries
- Seamless checkout process

### 🛠️ Developer Experience
- TypeScript for type safety
- Modular architecture
- Comprehensive error handling
- Easy local development setup

## Contributing

### Code Style
- Follow existing code conventions
- Use TypeScript for type safety
- Write meaningful commit messages
- Include tests for new features

### Pull Request Process
1. Fork the specific component repository
2. Create a feature branch
3. Make your changes with tests
4. Submit a pull request with detailed description

## Deployment

### Production Environment
- **Frontend**: Vercel or Netlify
- **Backend**: Railway, Heroku, or DigitalOcean
- **Database**: MongoDB Atlas
- **CDN**: Cloudinary for image optimization

### Environment Variables
Ensure all required environment variables are configured:
- Database connection strings
- JWT secrets
- API keys for third-party services
- Frontend/backend URLs

## Support

For questions or issues:
- Check the individual repository documentation
- Review the API documentation
- Contact the development team

## License

This project is proprietary software developed for RENART luxury jewelry platform.

---

**Built by the Bedirhan Tong**
