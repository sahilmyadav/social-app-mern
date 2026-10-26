# ClickMe — Social Media App (MERN Stack)

A full-stack social media application built with the MERN stack. The repository
contains a Node.js/Express backend API and a React frontend, with Docker and
nginx configuration for running the whole stack together.

## Features

- User accounts with authentication and profiles
- Social feed with posts and media
- Frontend built with React, Radix UI components and React Hook Form
- Backend with controllers, models, route schemas and middleware structure
- Test setup on the backend (Vitest) and linting on both sides

## Tech Stack

- **Frontend:** React, Radix UI, React Hook Form
- **Backend:** Node.js, Express, MongoDB
- **Infra:** Docker Compose, nginx, Render config (`render.yaml`)

## Getting Started

### With Docker

```bash
docker compose up --build
```

### Without Docker

```bash
# backend
cd backend
npm install
npm run dev

# frontend (new terminal)
cd frontend
npm install
npm run dev
```

Copy `.env.example` to `.env` and fill in your own values (MongoDB URI, JWT
secret, Firebase keys) before running. Never commit real keys.

## Project Structure

```
backend/    Express API (src, controllers, models, routes, tests)
frontend/   React app (clickme-social)
nginx/      Reverse proxy config
scripts/    Helper scripts
```

## Notes

This project was built for learning and portfolio purposes.
