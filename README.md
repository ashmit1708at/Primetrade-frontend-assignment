# Primetrade Frontend Developer Intern Assignment

Scalable Web App with Authentication & Dashboard (using Next.js + Tailwind + Node/Express backend)

## Project Description
Built a responsive React/Next.js frontend with JWT authentication, protected dashboard, tasks CRUD, search/filter, and integrated with a basic Node.js + MongoDB backend.

## Features Implemented
- Register / Login / Logout (JWT token)
- Protected Dashboard (only after login)
- Display user profile (email from JWT or API)
- Tasks CRUD (Create, Read, Update, Delete)
- Search and filter tasks
- Responsive design (Tailwind CSS)
- Client-side form validation (react-hook-form + Zod)
- Backend: Signup/Login, Profile, Tasks APIs, bcrypt hashing, JWT middleware

## Tech Stack
- Frontend: Next.js, Tailwind CSS, Axios, react-hook-form, Zod, jwt-decode
- Backend: Node.js, Express, Mongoose, JWT, bcrypt
- Database: MongoDB Atlas

## How to Run Locally
### Backend
cd backend
npm install
# Create .env with MONGO_URI and JWT_SECRET
npm run dev

### Frontend
cd frontend
npm install
npm run dev

Open http://localhost:3000

## API Endpoints (basic docs)
- POST /api/auth/register → {email, password}
- POST /api/auth/login → returns {token}
- GET /api/tasks → list user tasks (protected)
- POST /api/tasks → create task
- PUT /api/tasks/:id → update
- DELETE /api/tasks/:id → delete

Postman collection: See postman_collection.json in repo (upload kar dena)

## Production Scaling Note
- Frontend → Deploy on Vercel (free, auto HTTPS, fast)
- Backend → Deploy on Render/Railway (free tier)
- Use environment variables for secrets
- Add refresh tokens, rate limiting, HTTPS
- For high traffic: Redis caching, load balancer, separate microservices
- Monitoring: Add Sentry for errors

Thank you for reviewing my assignment!  
Ashmit  
Delhi, India
