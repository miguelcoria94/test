# TinyKr - URL Shortener Service

![TinyKr Logo](https://i.ibb.co/VrN0VZ1/01.png)

TinyKr is a full-featured URL shortening service built with the MERN stack. It allows users to create shortened links with custom aliases, track click analytics, and generate QR codes for their shortened URLs.

## 🚀 Features

- **URL Shortening**: Create short, easy-to-remember URLs for long links
- **Custom Aliases**: Choose your own custom short URL paths
- **QR Code Generation**: Automatically generate QR codes for all shortened links
- **Comprehensive Analytics**: Track clicks with detailed information:
  - Geographic location
  - Device types
  - Browser information
  - Operating systems
  - Time-based analytics
- **User Authentication**: Secure JWT-based authentication
- **Dashboard**: Visual analytics with charts and graphs
- **Expiration Dates**: Set custom expiration dates for URLs
- **Responsive UI**: Works on all devices with a modern, clean interface

## 💻 Tech Stack

### Backend

- **Node.js** & **Express.js** - Server framework
- **MongoDB** & **Mongoose** - Database and ODM
- **JWT** - Authentication
- **Geoip-lite** - IP geolocation for analytics
- **QRCode** - QR code generation
- **UA-Parser-JS** - User agent parsing for analytics

### Frontend

- **React 19** - UI library
- **React Router v7** - Client-side routing
- **React-ChartJS-2** - Data visualization
- **React-Toastify** - Notifications
- **Tailwind CSS** - Styling (via custom classes)

### Development & Deployment

- **Vite** - Build tool and development server
- **Jest** - Testing framework
- **MongoDB Memory Server** - Testing database
- **Heroku** - Deployment platform

## 📋 Installation & Setup

### Prerequisites

- Node.js (v18+)
- MongoDB (local installation or MongoDB Atlas account)
- npm or yarn

### Installation Steps

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/tinykr.git
   cd tinykr
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory with the following variables:

   ```
   DATABASE_URL=mongodb://localhost:27017/tinykr
   SECRET=your_jwt_secret_key
   BASE_URL=http://localhost:3001
   PORT=3001
   NODE_ENV=development
   ```

4. **Start the development server**

   ```bash
   npm run dev
   ```

   This will start both the backend server and the frontend development server concurrently.

5. **Build for production**

   ```bash
   npm run build
   ```

6. **Seed the database (optional)**
   ```bash
   npm run seed
   ```

## 🧪 Testing

```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch
```

## 🚀 Deployment

The application is configured for deployment on Heroku:

```bash
# Login to Heroku
heroku login

# Create a new Heroku app
heroku create your-app-name

# Add MongoDB add-on
heroku addons:create mongodb

# Push to Heroku
git push heroku main
```

## 🔮 Future Features

- **API Access**: Public API for URL shortening with token authentication
- **Teams & Sharing**: Collaborative URL management for teams
- **Advanced Analytics**: Heat maps, click path analysis, and conversion tracking
- **Custom Domains**: Support for user-provided custom domains
- **Password Protection**: Secure shortened URLs with password access
- **URL Bundles**: Group related URLs under a single umbrella
- **Link Rotation**: Rotate destination URLs based on rules (A/B testing)
- **Rate Limiting**: Protect against abuse with rate limiting
- **Enhanced QR Codes**: Customizable QR codes with branding options

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🙏 Acknowledgements

- [ShortID](https://github.com/dylang/shortid) - URL generation
- [QRCode](https://github.com/soldair/node-qrcode) - QR code generation
- [UA-Parser-JS](https://github.com/faisalman/ua-parser-js) - User agent parsing
- [React ChartJS 2](https://github.com/reactchartjs/react-chartjs-2) - Data visualization
