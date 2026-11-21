# Datheon Full Stack Web Development Internship

This repository collects the projects I built during my **Full Stack Web Development Internship at Datheon**. Each project lives in its own repository and is linked here as a Git submodule, so this repo works as a single index of all the internship tasks.

## Projects

**| Project | Repository | 
1. | --- | --- | --- |
2. | Task Manager | [Task_Manager](https://github.com/danishfarooq737/Task_Manager) 
3. | DF Store Website | [DF-Store-Website](https://github.com/danishfarooq737/DF-Store-Website) 
4. | DF Portfolio | [DF-Portfolio](https://github.com/danishfarooq737/DF-Portfolio) 
5. | Weather App | [Weather_app](https://github.com/danishfarooq737/Weather_app) 
**
---

## 1. Task Manager

A full-stack task management app with user authentication and per-user tasks.

**Features**
- Register, log in, and stay signed in with secure HttpOnly cookie authentication
- Create, view, update, and delete tasks
- Versioned REST API (`/api/v1`) with health, auth, and task routes

**Tech stack**
- **Frontend:** React + Vite, deployed on Vercel
- **Backend:** Node.js, Express, MongoDB (Mongoose), deployed on Render
- **Security:** Helmet, strict CORS allow-list, rate limiting, NoSQL injection and XSS sanitization, request body size limits
- **Logging:** Morgan + Winston

**API overview**

| Route | Purpose |
| --- | --- |
| `GET /api/v1/health` | Service health check |
| `/api/v1/auth/*` | Registration, login, current user |
| `/api/v1/tasks/*` | Task CRUD |

**Environment variables (backend)**

```env
NODE_ENV=production
API_PREFIX=/api/v1
CORS_ORIGIN=https://your-frontend.vercel.app
MONGO_URI=your-mongodb-connection-string
JWT_SECRET=your-secret
```

**Environment variables (frontend)**

```env
VITE_API_URL=https://your-backend.onrender.com/api/v1
```

---

## 2. DF Store Website

An online store front end for browsing products.

- Product listing and product detail views
- Responsive layout for mobile and desktop
- _Add: cart, checkout, backend, database, or payment details if included_

---

## 3. DF Portfolio

My personal portfolio website.

- About me, skills, projects, and contact sections
- Responsive, fast-loading design
- Links to the projects in this repository

---

## 4. Weather App

A weather app where users search for a city and see current conditions.

- City search with current temperature and conditions
- Data from a public weather API
- _Add: forecast, units toggle, or geolocation if included_

---

## Cloning with submodules

```bash
git clone --recurse-submodules https://github.com/danishfarooq737/Datheon_Full_Stack_Web_Development_Internship.git
```

If you already cloned without submodules:

```bash
git submodule update --init --recursive
```

To pull the latest changes from every project:

```bash
git submodule update --remote --merge
```

## Skills practiced

- HTML, CSS, JavaScript, React
- Node.js, Express, REST API design
- MongoDB and data modeling
- Authentication, security best practices, and CORS
- Git, GitHub, submodules, and deployment (Vercel, Render)

## Author

**Danish Farooq**
GitHub: [@danishfarooq737](https://github.com/danishfarooq737)
