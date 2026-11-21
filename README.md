# TaskFlow

Task management application with subtasks, priorities, and categories. Built with React and Express.

[![Node.js](https://img.shields.io/badge/Node.js-18+-green.svg)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-18-blue.svg)](https://reactjs.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## Description

TaskFlow is a task management application for developers and teams. It offers rich task metadata, priority sorting, subtasks, categories, bulk operations, dark/light themes, real-time search, and a progress dashboard. The backend is a RESTful API ready for database integration. Docker support is included for containerized deployment.

## Features

- Rich task metadata: titles, descriptions, due dates, custom tags
- Priority system with automatic sorting (High → Medium → Low)
- Subtasks to break complex tasks into trackable steps
- Categories for work, personal, and custom projects
- Bulk operations: complete, archive, or delete multiple tasks
- Dark/Light themes
- Real-time search across all task fields
- Progress dashboard with visual statistics
- Responsive design for desktop, tablet, and mobile
- Optimistic updates for instant feedback
- RESTful API with clean, documented endpoints
- Docker support with docker-compose

## Requirements

- Node.js >= 18
- npm or yarn
- Docker (optional, for containerized deployment)

## Installation

```bash
git clone https://github.com/NGeff/taskflow.git
cd taskflow
```

Backend:

```bash
cd backend
npm install
```

Frontend:

```bash
cd ../frontend
npm install
```

## Usage

Development — terminal 1 (API at `http://localhost:5000`):

```bash
cd backend
npm run dev
```

Development — terminal 2 (client at `http://localhost:5173`):

```bash
cd frontend
npm run dev
```

### Using Docker

```bash
docker-compose up -d
```

The API runs on port 5000 and the client on port 3000.

### Build

Frontend:

```bash
cd frontend
npm run build
```

Serve the `dist/` folder with Nginx or any static server.

### Tests

Backend:

```bash
cd backend
npm test
npm run test:coverage
```

Frontend:

```bash
cd frontend
npm test
npm run test:coverage
```

### Lint

Backend:

```bash
cd backend
npm run lint
npm run lint:fix
```

Frontend:

```bash
cd frontend
npm run lint
npm run lint:fix
```

## Project Structure

```
taskflow/
├── docker-compose.yml
├── backend/
│   ├── Dockerfile
│   ├── package.json
│   └── src/
│       └── index.js
├── frontend/
│   ├── Dockerfile
│   ├── index.html
│   ├── package.json
│   ├── vite.config.js
│   ├── tailwind.config.js
│   ├── postcss.config.js
│   └── src/
│       └── ...
└── README.md
```

## License

MIT © NGeff
