# OctoFit Tracker

A modern multi-tier fitness tracking application built with React 19, Node.js/Express, and MongoDB.

## Architecture

### Frontend
- **Framework**: React 19
- **Build Tool**: Vite
- **Port**: 5173
- **Features**: Component-based UI for fitness tracking

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Language**: TypeScript
- **Port**: 8000
- **Database**: MongoDB with Mongoose ODM

### Database
- **System**: MongoDB
- **Port**: 27017
- **Connection String**: `mongodb://localhost:27017/octofit-tracker`

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite application
│   ├── src/
│   │   ├── main.jsx
│   │   ├── App.jsx
│   │   └── index.css
│   ├── package.json
│   └── vite.config.js
├── backend/           # Express.js + TypeScript API
│   ├── src/
│   │   └── index.ts
│   ├── package.json
│   └── tsconfig.json
└── README.md
```

## Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB running on localhost:27017

### Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

Frontend will run at `http://localhost:5173`

### Backend Setup

```bash
cd octofit-tracker/backend
npm install
cp .env.example .env
npm run dev
```

Backend will run at `http://localhost:8000`

### Database Setup

Ensure MongoDB is running on port 27017:

```bash
mongod --port 27017
```

## API Endpoints

- `GET /api/health` - Health check endpoint

## Development

### Frontend Commands
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

### Backend Commands
- `npm run dev` - Start development server with hot reload
- `npm run build` - Compile TypeScript to JavaScript
- `npm run start` - Run compiled backend

## Port Configuration

- **Frontend**: 5173
- **Backend API**: 8000
- **MongoDB**: 27017

## Next Steps

1. Create User and Workout models in MongoDB
2. Build API endpoints for CRUD operations
3. Create React components for UI
4. Add authentication and authorization
5. Deploy to production
