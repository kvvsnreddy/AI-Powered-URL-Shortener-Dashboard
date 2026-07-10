# AI-Powered URL Shortener Dashboard

## Overview

AI-Powered URL Shortener Dashboard is a full-stack web application that allows users to shorten long URLs, generate AI-powered custom aliases, track click analytics, and manage links through an interactive dashboard.

The application combines URL shortening, analytics, authentication, QR code generation, and AI-powered alias suggestions into a single platform.

---

## Features

- User Registration & Login (JWT Authentication)
- Shorten Long URLs
- AI-Based Custom Alias Generation
- Redirect Short URLs
- Click Tracking
- QR Code Generation
- Analytics Dashboard
- Search & Filter URLs
- Delete URLs
- Responsive UI

---

## Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Axios
- Chart.js

### Backend
- FastAPI
- Python
- SQLAlchemy
- JWT Authentication

### Database
- SQLite (Development)
- PostgreSQL (Production)

### AI
- OpenAI API (for alias generation)

---

## Project Structure

```
AI-URL-Shortener/
│
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── database.py
│   │   ├── models.py
│   │   ├── schemas.py
│   │   ├── auth.py
│   │   ├── routes.py
│   │   ├── services.py
│   │   └── utils.py
│   │
│   ├── requirements.txt
│   └── .env
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

---


### Authentication

```
POST /register

POST /login
```

### URL

```
POST /shorten

GET /{short_code}

DELETE /url/{id}

GET /dashboard
```

### Analytics

```
GET /analytics/{id}
```

---

## Database Tables

### Users

| Field | Type |
|-------|------|
| id | Integer |
| username | String |
| email | String |
| password | String |

---

### URLs

| Field | Type |
|-------|------|
| id | Integer |
| original_url | Text |
| short_code | String |
| created_at | DateTime |
| user_id | Integer |

---

### Clicks

| Field | Type |
|-------|------|
| id | Integer |
| url_id | Integer |
| ip_address | String |
| browser | String |
| clicked_at | DateTime |

---

AI Suggestion

```
iphone16

apple-phone

amazon-iphone
```

---

## Dashboard

Displays

- Total URLs
- Total Clicks
- Top Performing Links
- Daily Clicks
- Monthly Clicks
- QR Codes
- Recent Activity

---

## Security

- JWT Authentication
- Password Hashing (bcrypt)
- Input Validation
- SQL Injection Protection
- CORS Support

---

## Future Enhancements

- Custom Domains
- Expiring URLs
- Team Collaboration
- Bulk URL Import
- AI Click Prediction
- Geo-location Analytics
- Mobile Application

---

## Learning Outcomes

- Full Stack Development
- REST API Design
- Authentication
- SQL Database Design
- AI API Integration
- Data Visualization
- QR Code Generation
- Deployment using Docker

---



B.Tech Computer Science Engineering

Python | FastAPI | React | SQL | AI
