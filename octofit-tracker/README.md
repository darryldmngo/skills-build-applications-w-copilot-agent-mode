# OctoFit Tracker

A modern multi-tier application for fitness tracking, built with React 19, Node.js/Express, and MongoDB.

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite application
│   ├── src/
│   ├── package.json
│   ├── vite.config.ts
│   └── tsconfig.json
└── backend/           # Node.js + Express + TypeScript API
    ├── src/
    ├── package.json
    └── tsconfig.json
```

## Technology Stack

### Frontend
- **React 19** - UI library
- **Vite** - Build tool and dev server
- **TypeScript** - Type safety
- **Port:** 5173

### Backend
- **Node.js** - Runtime
- **Express** - Web framework
- **TypeScript** - Type safety
- **Mongoose** - MongoDB ODM
- **Port:** 8000

### Database
- **MongoDB** - Database
- **Port:** 27017

## Getting Started

### Prerequisites
- Node.js 18+
- MongoDB running locally or connection string

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
npm run dev
```

Backend will be available at `http://localhost:8000`

### MongoDB Setup

Ensure MongoDB is running on the default port 27017:

```bash
# On macOS with Homebrew
brew services start mongodb-community

# On Linux
sudo systemctl start mongod

# Or run with Docker
docker run -d -p 27017:27017 --name mongodb mongo:latest
```

## API Endpoints

- `GET /api/health` - Health check endpoint

## Development

### Frontend Development
- Run `npm run dev` for hot module reloading
- Run `npm run build` to create production build

### Backend Development
- Run `npm run dev` with tsx watch for auto-reload
- Run `npm run build` to compile TypeScript
- Run `npm start` to run compiled JavaScript

## Environment Variables

Create a `.env` file in the backend directory:

```env
MONGODB_URI=mongodb://localhost:27017/octofit-tracker
PORT=8000
NODE_ENV=development
```
