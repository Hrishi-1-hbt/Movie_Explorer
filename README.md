# 🎬 Movie Explorer

A full-stack movie exploration application built with React and Node.js, powered by the OMDB API.

![OMDB Explorer](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![UI](https://img.shields.io/badge/UI-Premium-ff0a54.svg)
![Animations](https://img.shields.io/badge/Animations-60FPS-00d9ff.svg)

## ✨ Features

### Frontend
- 🎨 **Rich UI/UX** - Glassmorphism design with 60 FPS animations
- 🔍 **Advanced Search** - Search movies by title with filters (year, type)
- 📱 **Responsive Design** - Works seamlessly on all devices
- ❤️ **Favorites System** - Save and manage favorite movies
- 📄 **Pagination** - Navigate through large result sets
- 🎭 **Movie Details** - Comprehensive information with ratings and cast

### Backend
- 🚀 **RESTful API** - Clean, well-structured endpoints
- 💾 **Smart Caching** - In-memory cache with optional Redis support
- 🔒 **Security** - Rate limiting, CORS, and Helmet protection
- 🎯 **Error Handling** - Comprehensive logging and validation
- 🔑 **API Integration** - Secure OMDB API key management

---

## 🏗️ Architecture

```
omdb-movie-explorer/
├── backend/               # Node.js/Express API
│   ├── controllers/       # Request handlers
│   ├── middleware/        # Custom middleware
│   ├── routes/           # API routes
│   ├── services/         # Business logic
│   │   ├── omdbService.js      # OMDB API integration
│   │   └── cacheService.js     # Caching layer
│   └── server.js         # Application entry point
│
└── frontend/             # React application
    ├── src/
    │   ├── components/   # Reusable components
    │   ├── pages/        # Page components
    │   ├── services/     # API client
    │   ├── hooks/        # Custom hooks
    │   └── App.jsx       # App root
    └── public/           # Static assets
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- OMDB API Key (Get free key at [https://www.omdbapi.com/apikey.aspx](https://www.omdbapi.com/apikey.aspx))
- Redis (optional, for distributed caching)

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/GMahesh007/Movie_Explorer_.git
cd omdb-movie-explorer
```

2. **Setup Backend**

```bash
cd backend
npm install

# Create .env file from example
copy .env.example .env
```

Edit `.env` and add your OMDB API key:

```env
OMDB_API_KEY=your_actual_api_key_here
PORT=5000
NODE_ENV=development
CACHE_TTL=3600
CACHE_MAX_SIZE=1000
USE_REDIS=false
```

3. **Setup Frontend**

```bash
cd ../frontend
npm install
```

### Running the Application

**Option 1: Run Both Servers Separately**

Terminal 1 (Backend):

```bash
cd backend
npm start
# or for development with auto-reload:
npm run dev
```

Terminal 2 (Frontend):

```bash
cd frontend
npm run dev
```

**Option 2: Build and Deploy**

Build frontend:

```bash
cd frontend
npm run build
```

The application will be available at:

- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## 📝 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

- [OMDB API](https://www.omdbapi.com/) - Movie database
- [React](https://reactjs.org/) - Frontend framework
- [Express](https://expressjs.com/) - Backend framework

---

**Built with ❤️ for Movie Enthusiasts**
