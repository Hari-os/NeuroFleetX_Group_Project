# NeurofleetX

NeurofleetX is a prototype fleet-management web application combining a Java backend and a React + TypeScript frontend. It includes pages and tools for real-time vehicle monitoring, maintenance, bookings, emergency management, and an AI control center.

This repository contains multiple demos and exercises alongside the main application. The primary app is under `backend/` (Java, Maven) and `frontend/` (Vite + React + TypeScript).

Quick Links
- Backend: `backend/` (Maven + Spring Boot)
- Frontend: `frontend/` (Vite + React + TypeScript)
- DB schema: `backend/database-schema.sql`

Features
- Dashboard and system health
- Live map and vehicle tracking
- Fleet management and maintenance pages
- Booking system and emergency management
- AI Control Center page (demo)

Tech stack
- Backend: Java, Spring Boot (Maven)
- Frontend: React, TypeScript, Vite, Tailwind CSS
- Database: SQL (schema in `backend/database-schema.sql`)

Prerequisites
- Java 17+ and Maven for the backend
- Node.js 16+ (recommended Node 18+) and `npm` for the frontend
- A SQL database to run the schema (Postgres / MySQL or other)

Quickstart (development)
Open two terminals (PowerShell recommended) — one for backend, one for frontend.

Backend (from repository root):

```
cd backend
mvn clean install
mvn spring-boot:run
```

The backend runs on the port configured in the Spring Boot configuration (check `src/main/resources` or `target/classes/application.properties` if present).

Frontend (from repository root):

```
cd frontend
npm install
npm run dev
```

The frontend uses Vite and will typically serve at `http://localhost:5173` by default.

Production build
Backend:

```
cd backend
mvn clean package
java -jar target/*.jar
```

Frontend:

```
cd frontend
npm run build
npm run preview    # or serve the `dist/` folder with any static server
```

Database
If you need to initialize a database, run the SQL in `backend/database-schema.sql` against your database engine. Adjust connection settings in the backend application's configuration.

Project structure
- `backend/` — Java backend application (Maven)
- `frontend/` — React + TypeScript frontend (Vite)
- `JavaExercises/`, `ReactExercises/`, `loginpage/` — example/demo projects and exercises

Contributing
Contributions are welcome. Create issues for bugs or feature requests and open pull requests with clear descriptions and minimal, focused changes.

License
This repository does not include a license file. Add a license if you intend to open source the project.

