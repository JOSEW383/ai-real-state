# AI Real Estate 🏠

A modern real estate platform that uses Artificial Intelligence to help users find their ideal property. The application consists of a frontend built with React and a backend for property management and recommendations.

<p><img src="https://github.com/JOSEW383/ai-real-state/blob/master/AiRealStateAnalyzerDemo.gif" alt="Demo" width="50%" height="50%" /></p>

## 🚀 Technologies Used

### Frontend
- React with TypeScript
- Vite for fast development and optimized builds
- Tailwind CSS for responsive design
- i18n for internationalization (English/Spanish)
- Supabase for database and authentication
- PWA (Progressive Web App) for enhanced mobile experience
- Context API for state management
- Lucide React for iconography

### Backend
- Python with FastAPI
- FastAPI CORS middleware for cross-origin request handling
- Uvicorn as a high-performance ASGI server
- PostgreSQL through Supabase
- Web Scraping using cheerio and axios
- Docker for containerization
- AI usage for data analysis and rating generation

### Integration and DevOps
- Docker Compose for orchestrating services
- Continuous integration between frontend and backend
- Optimized production environment with Dockerfile
- Environment variables for flexible configuration

## 📋 Prerequisites

- Node.js (v16 or higher recommended)
- Python 3.9 or higher
- Docker and Docker Compose
- Supabase account and project

## 🛠️ Installation and Setup

1. Clone the repository:
```bash
git clone https://github.com/josew383/ai-real-state.git
cd ai-real-state
git submodule update --init --recursive
```

2. To update the repository with the latest changes:
```bash
git pull && git submodule update --init --recursive --remote
```

3. Frontend setup:
```bash
cd airs-front
npm install
cp .env.example .env  # Configure the variables according to your credentials
```

4. Backend setup:
```bash
cd airs-back
pip install -r requirements.txt
cp .env.example .env  # Configure the variables according to your credentials
```

## 🚀 Running the Application

### Using Docker Compose (Recommended)
The complete application can be started using Docker Compose:
```bash
docker-compose up -d
```

### Manual Setup for Development

1. Start the backend:
```bash
cd airs-back
./start_server.sh
```

2. Start the frontend:
```bash
cd airs-front
npm run dev
```

## 🔗 Frontend-Backend Integration

The frontend communicates with the backend through a REST API implemented with FastAPI:

- The frontend uses axios to make HTTP requests to the backend
- CORS is configured in the backend to allow requests from the frontend
- Authentication is handled using Supabase JWT tokens
- The backend endpoints provide functionalities for:
  - Authentication and user management
  - Property CRUD operations
  - Shared catalog management
  - Web scraping from real estate portals
  - Property analysis and scoring

## 🤖 Artificial Intelligence Integration

This project leverages cutting-edge AI technologies to revolutionize the real estate search experience:

### AI-Powered Development
- GitHub Copilot for programming assistance throughout the development process
- Generation of React components and API endpoints through AI pair programming
- SQL query optimization and data modeling enhanced by AI recommendations
- Automated testing pattern suggestions and code refactoring

## 🌟 Functional Features

### Property Management
- Adding and removing properties
- Automatic scraping from real estate portals
- Detailed visualization with image gallery
- Data export in PDF and JSON formats
- Advanced filtering and sorting

### Shared Catalogs
- Creation and management of property collections
- Collaboration between multiple users
- Access control and permissions
- Sharing catalogs through unique identifiers

### User Management
- Registration and login with email
- Customizable user profiles
- Saved property preferences
- History of visited properties

### User Experience
- Responsive design for mobile and desktop
- Dark/light mode with automatic detection
- Multi-language support (Spanish and English)
- Installable PWA interface on mobile devices

## 🔒 Security
- Secure authentication through Supabase Auth
- Environment variables for secrets
