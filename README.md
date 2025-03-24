# Realtime Chat Application

A real-time chat application built with Django.

## Setup Instructions

### Prerequisites
- Python 3.x
- pip (Python package installer)

### Project Setup

1. Create and activate virtual environment:
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment (Windows)
.\venv\Scripts\activate
```

2. Install required packages:
```bash
pip install django
```

3. Create Django project:
```bash
django-admin startproject chatire .
```

4. Run database migrations:
```bash
python manage.py migrate
```

5. Start the development server:
```bash
python manage.py runserver
```

The application will be available at http://127.0.0.1:8000/

## Project Structure
```
Realtime-Chat-application/
├── manage.py
├── chatire/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── venv/
```

## Development
- The development server automatically reloads when code changes are detected
- To stop the server, press Ctrl+C in the terminal
- To deactivate the virtual environment, type `deactivate` in the terminal

## Next Steps
1. Create a new app for chat functionality
2. Set up user authentication
3. Implement real-time chat features
4. Add styling and frontend components 