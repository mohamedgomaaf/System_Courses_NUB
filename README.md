# Full Stack Project

This project consists of a **client** (Next.js (React.js) app) and a **server** (Node.js/Express or similar backend) in a monorepo-style setup.

## Project Structure

```
.
├── client/      # Next.js frontend
├── server/      # Node.js backend (API, services, etc.)
└── README.md    # Root README
```

---

## Getting Started

These instructions will help you set up and run the project locally.

### Prerequisites

Ensure you have the following installed:

* [Node.js](https://nodejs.org/) (v18 or later recommended)
* [npm](https://www.npmjs.com/) (comes with Node.js)
* [mongodb](https://www.mongodb.com/try/download/community)
* [mongodb compass](https://www.mongodb.com/try/download/compass)

---

## Client Setup (Next.js)

Navigate to the `client` directory and install dependencies:

```bash
cd client
npm install
```

To run the development server:

```bash
npm run dev
```

This will start the Next.js app at [http://localhost:3000](http://localhost:3000).

---

## Server Setup (Node.js)

Navigate to the `server` directory and install dependencies:

```bash
cd server
npm install
```

To run the server in development mode (with `nodemon`):

```bash
npm run dev
```

This will start the backend server, typically at [http://localhost:5000](http://localhost:5000) or a configured port.

---

## 🛠 Project Scripts

You’ll find common commands in the `package.json` of each part. Here are some examples:

### Client

* `npm run dev` — Start development server
* `npm run build` — Build for production
* `npm run start` — Start production server

### Server

* `npm run dev` — Start development backend (with live reload)
* `npm run start` — Start production backend

---

## 📦 Environment Variables

Create `.env` files in both `client/` and `server/` directories as needed. These should define variables like API URLs, secrets, and database connections.

Example for `server/.env`:

```
PORT=5000
NODE_ENV=development
MONGODB_URI=your_database_url
```
