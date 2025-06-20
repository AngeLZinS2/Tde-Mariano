# ONG Website Project

## Overview
A web application for managing donations and campaigns for an NGO, built with:
- Angular 19 frontend
- Python Flask backend
- SQLite database

## Features
- User authentication (login/register)
- Campaign management
- Donation processing
- Admin dashboard
- User profiles

## Technical Stack

### Frontend
- Angular 19
- Angular Material
- RxJS
- ngx-mask

### Backend
- Python Flask
- SQLite database
- JWT authentication
- bcrypt password hashing

## Development Setup

### Prerequisites
- Node.js (v18+)
- Python 3.8+
- npm

### Installation
1. Clone repository
2. Install dependencies:
```bash
npm install
```

3. Start development server:
```bash
npm run start
```

## Backend Setup

1. Navigate to backend folder:
```bash
cd backend
```

2. Install dependencies:
```bash
python -m pip install -r requirements.txt
```

3. Start server:
```bash
python app.py
```

The server will run on port 5000 (http://localhost:5000).

## API Documentation

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get current user
- `PUT /api/auth/update-profile` - Update profile
- `PUT /api/auth/change-password` - Change password

### Campaigns
- `GET /api/campaigns` - List all campaigns
- `POST /api/campaigns` - Create campaign
- `PUT /api/campaigns/:id` - Update campaign
- `DELETE /api/campaigns/:id` - Delete campaign (admin only)

### Donations
- `POST /api/donations` - Make donation
- `GET /api/donors` - List donors

### Admin
- `GET /api/admin/users` - List all users
- `GET /api/admin/stats` - Get system statistics
- `PUT /api/admin/users/:id/toggle-admin` - Toggle admin status

## Database Schema
![Database Schema](https://images.pexels.com/photos/669615/pexels-photo-669615.jpeg)

## Environment Variables
Create `.env` or `env.local` file with:
```
JWT_SECRET=your-secret-key
```

## Deployment
To build the application:
```bash
npm run build
```

## License
MIT
