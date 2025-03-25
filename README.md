# Chatire - Real-time Chat Application

A real-time chat application built with Django REST framework and Vue.js.

## Technologies Used

### Backend
- Django 5.1.7
- Django REST Framework 3.15.2
- Django REST Framework SimpleJWT
- Djoser (for authentication)
- Django CORS Headers

### Frontend
- Vue.js 2.x
- Bootstrap 4
- jQuery
- Webpack

## Project Structure
```
chatire/
├── backend/
│   ├── chatire/          # Django project settings
│   ├── manage.py
│   └── requirements.txt
│
└── frontend/
    ├── src/
    │   ├── components/   # Vue components
    │   ├── router/       # Vue router configuration
    │   └── App.vue       # Root component
    └── index.html        # Frontend entry point
```

## Setup Instructions

### Backend Setup
1. Create and activate virtual environment:
```bash
python -m venv venv
source venv/Scripts/activate  # Windows
source venv/bin/activate      # Linux/Mac
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run migrations:
```bash
python manage.py migrate
```

4. Start Django development server:
```bash
python manage.py runserver
```

The backend server will be available at http://localhost:8000

### Frontend Setup
1. Navigate to frontend directory:
```bash
cd chatire-frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start development server:
```bash
npm run dev
```

The frontend application will be available at http://localhost:8080

## API Endpoints

### Authentication Endpoints
- POST `/auth/users/` - Register new user
- POST `/auth/token/login/` - Login user (get token)
- POST `/auth/token/logout/` - Logout user
- GET `/auth/users/me/` - Get current user details

## Features
- User registration and authentication
- Token-based authentication
- Real-time chat functionality (coming soon)
- Responsive UI with Bootstrap 4

## Development
- Backend API is configured with CORS to accept requests from frontend
- Authentication is handled using Djoser and Token Authentication
- Frontend uses Vue Router for navigation and route protection

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request 