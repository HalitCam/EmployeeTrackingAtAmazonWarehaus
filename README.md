# Amazon Lager
Ziel = In diesem Web-Aplikation versucht man die Tasken auf Mitarbeiter als übe digital platform zu verteilen. Und nach dem Zeitraum (monatlich, täglich, ...) werden die Leistungen des Lagers und der Mitarbeiter angezeigt.<br/>

The goal is to distribute tasks to employees via a comprehensive digital platform. Warehouse and employee performance will then be monitored over a specific period (monthly, daily, etc.). <br/>
## Stack

- Frontend: React
- Backend: Node.js + Express
- Database: MongoDB
- Cache: Redis
- Containers: Docker Compose

## Quick Start (Docker)

1. Make sure Docker is installed.
2. From the project root, run:

```bash
docker compose up --build
```

3. Open:
- Client: http://localhost:3000
- API: http://localhost:4000

## Local Development (Without Docker)

### 1) Backend

Create `backend/.env`:

```env
MONGO_URI=mongodb://localhost:27018/amazon-lager
JWT_SECRET=your_jwt_secret
JWT_REFRESH_SECRET=your_jwt_refresh_secret
```

Then run:

```bash
cd backend
npm install
npm run dev
```

### 2) Client

```bash
cd client
npm install
npm start
```

## Notes

- Backend runs on port `4000`.
- Client runs on port `3000`.
- Docker Compose starts MongoDB and Redis automatically.

## Screenshots of Web-APP
### Homepage
![Home Page](./images/shot1.png)
### Dashboard of Admin 
![Dashboard](./images/shot2.png)
### To build a task
![building](./images/shot4.png)
### Tasks to review
![Tasks](./images/shot3.png)
### Taking over tasks by employee
![Employee](./images/shot5.png)
### The following of Tasks
![Following](./images/shot6.png)
### The following of performance
![Following](./images/shot7.png)
### The following performance of employee
![Following](./images/shot8.png)
