# OctoFit Tracker

A modern multi-tier fitness tracking application built with React 19, Node.js + Express, and MongoDB.

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite (Port 5173)
│   ├── src/
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
└── backend/           # Node.js + Express + TypeScript (Port 8000)
    ├── src/
    ├── package.json
    ├── tsconfig.json
    └── .env.example
```

## Technology Stack

### Frontend
- **React 19** - Latest React version
- **Vite** - Modern frontend build tool
- **JavaScript/JSX** - Component development
- **CSS** - Styling

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **TypeScript** - Type safety
- **Mongoose** - MongoDB ODM
- **CORS** - Cross-origin resource sharing
- **dotenv** - Environment variables

### Database
- **MongoDB** - NoSQL database (Port 27017)

## Port Configuration

- **Frontend:** `5173`
- **Backend API:** `8000`
- **MongoDB:** `27017`

## Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB running locally or remotely
- npm or yarn

### Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

Frontend will be available at `http://localhost:5173`

### Backend Setup

```bash
cd octofit-tracker/backend
npm install

# Create .env file from .env.example
cp .env.example .env

# Development
npm run dev

# Build
npm run build

# Production
npm start
```

Backend API will be available at `http://localhost:8000`

## Available API Endpoints

- `GET /api/health` - Health check endpoint

## Development Workflow

1. Start MongoDB
2. Run backend development server: `npm run dev` (from backend directory)
3. Run frontend development server: `npm run dev` (from frontend directory)
4. Open browser to `http://localhost:5173`

## Building for Production

### Frontend
```bash
cd octofit-tracker/frontend
npm run build
```

### Backend
```bash
cd octofit-tracker/backend
npm run build
npm start
```

## License

MIT
