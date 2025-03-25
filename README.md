# MERN Bug Tracker

## Overview
A simple Bug Tracker application built with the **MERN** (MongoDB, Express, React, Node.js) stack. This application allows users to report, track, and manage bugs in a project.

## Features
- **Report Bugs**: Users can create new bug reports.
- **View Bugs**: List of all reported bugs.
- **Update Bug Status**: Change status (e.g., Open, In-Progress, Resolved).
- **Delete Bugs**: Remove bugs from the system.

## Tech Stack
- **Backend**: Node.js, Express.js, MongoDB
- **Frontend**: React, Vite
- **Testing**: Jest, Supertest, React Testing Library

## Installation

### Prerequisites
Ensure you have the following installed:
- Node.js (v18+ recommended)
- MongoDB (local or Atlas)
- Git

### Backend Setup
```sh
# Clone the repository
git clone https://github.com/yourusername/mern-bug-tracker.git
cd mern-bug-tracker/backend

# Install dependencies
npm install

# Set environment variables (.env)
VITE_API_URL=http://localhost:5000
MONGO_URI=<your-mongodb-connection-string>
PORT=5000

# Start the server
npm run dev
```

### Frontend Setup
```sh
cd ../frontend

# Install dependencies
npm install

# Start the development server
npm run dev
```
The frontend will be available at `http://localhost:5173`.

## API Routes

### Bugs API (Backend)
| Method | Endpoint          | Description           |
|--------|------------------|-----------------------|
| GET    | `/api/bugs`      | Get all bugs         |
| POST   | `/api/bugs`      | Create a new bug     |
| PATCH  | `/api/bugs/:id`  | Update bug status    |
| DELETE | `/api/bugs/:id`  | Delete a bug         |

## Running Tests
### Backend Tests
```sh
cd backend
npm test
```
### Frontend Tests
```sh
cd frontend
npm test
```

## Debugging
Use the following command to start debugging the backend:
```sh
node --inspect server.js
```
Then open `chrome://inspect` in your browser.

## Error Handling
- **Backend**: Express middleware handles errors gracefully.
- **Frontend**: React error boundaries prevent crashes from affecting the whole UI.

## Contributing
1. Fork the repo
2. Create a feature branch (`git checkout -b feature-name`)
3. Commit changes (`git commit -m "Add feature"`)
4. Push to branch (`git push origin feature-name`)
5. Open a Pull Request

## License
This project is open-source under the **MIT License**.

