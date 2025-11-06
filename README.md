# Stock Market Analysis and Prediction System

A full-stack web application for stock market analysis, prediction, and recommendations using Django (Python) backend and React frontend.

## Features

- **Stock Data Analysis**: View and analyze historical stock data
- **Price Prediction**: AI-powered stock price prediction
- **Recommendation System**: Get personalized stock recommendations
- **Interactive Dashboard**: User-friendly interface for data visualization
- **API Integration**: Seamless integration with stock market data providers

## Tech Stack

### Backend
- **Framework**: Django 5.1.7
- **Database**: PostgreSQL
- **AI/ML**: Google Gemini API
- **API**: Django REST Framework
- **Authentication**: JWT (JSON Web Tokens)

### Frontend
- **Framework**: React.js
- **UI Components**: Custom components with TailwindCSS
- **State Management**: React Context API
- **Data Visualization**: Chart.js
- **Build Tool**: Vite

## Prerequisites

- Python 3.8+
- Node.js 16+
- PostgreSQL 12+
- npm or yarn

## Getting Started

### Backend Setup

1. Clone the repository
2. Navigate to the backend directory:
   ```bash
   cd django_backend_for_bot_json-main
   ```
3. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   .\venv\Scripts\activate  # On Windows
   ```
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Set up environment variables (create `.env` file):
   ```env
   DATABASE_URL=postgresql://postgres:your_password@localhost:5432/your_database
   GEMINI_API=your_gemini_api_key
   SECRET_KEY=your_django_secret_key
   DEBUG=True
   ```
6. Run migrations:
   ```bash
   python manage.py migrate
   ```
7. Start the development server:
   ```bash
   python manage.py runserver
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd ../client_recursion_6.0-main
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file:
   ```env
   VITE_API_URL=http://localhost:8000
   VITE_GEMINI_API=your_gemini_api_key
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

## Project Structure

```
Recursion6.0_2025/
├── client_recursion_6.0-main/    # Frontend React application
│   ├── src/                     # React source code
│   ├── public/                  # Static files
│   └── package.json             # Frontend dependencies
│
└── django_backend_for_bot_json-main/  # Backend Django application
    ├── stockmaster/             # Main Django project
    │   ├── api/                 # API endpoints
    │   ├── backend/             # Core backend logic
    │   ├── prediction/          # ML prediction models
    │   └── settings.py          # Django settings
    └── requirements.txt          # Python dependencies
```

## API Documentation

API documentation is available at `http://localhost:8000/api/docs/` when the backend server is running.

## Environment Variables

### Backend
- `DATABASE_URL`: PostgreSQL connection string
- `GEMINI_API`: Google Gemini API key
- `SECRET_KEY`: Django secret key
- `DEBUG`: Set to `False` in production

### Frontend
- `VITE_API_URL`: Backend API URL (default: `http://localhost:8000`)
- `VITE_GEMINI_API`: Google Gemini API key (if used in frontend)

## Contributing

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any queries, please contact the project maintainers.
