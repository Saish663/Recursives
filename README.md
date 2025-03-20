# Health Monitor System

A comprehensive health monitoring system that leverages wearable devices and AI to detect early signs of chronic diseases.

## Features

- Real-time health data collection from wearable devices (Apple Watch, Wear OS)
- Continuous health monitoring and anomaly detection
- AI-powered risk prediction for chronic diseases
- Real-time alerts and notifications
- Interactive dashboard for health metrics visualization
- Mobile app for on-the-go monitoring

## Tech Stack

### Backend
- FastAPI (Python)
- PostgreSQL
- WebSockets
- Machine Learning (scikit-learn, XGBoost, TensorFlow)

### Frontend
- React (Vite)
- ShadCN + TailwindCSS
- Recharts
- Firebase

### Mobile
- React Native (Expo)
- NativeWind
- Victory Native

## Setup Instructions

### Prerequisites
- Python 3.8+
- Node.js 16+
- PostgreSQL
- Firebase account
- Wearable device (Apple Watch or Wear OS device)

### Backend Setup

1. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
cd backend
pip install -r requirements.txt
```

3. Set up environment variables:
Create a `.env` file in the backend directory with:
```
DATABASE_URL=postgresql://postgres:postgres@localhost:5432/health_monitor
SECRET_KEY=your_secret_key
FIREBASE_CREDENTIALS=path/to/firebase-credentials.json
```

4. Initialize the database:
```bash
python init_db.py
```

5. Run the backend server:
```bash
uvicorn main:app --reload
```

### Frontend Setup

1. Install dependencies:
```bash
cd frontend
npm install
```

2. Set up environment variables:
Create a `.env` file in the frontend directory with:
```
VITE_API_URL=http://localhost:8000
VITE_FIREBASE_CONFIG=your_firebase_config
```

3. Run the development server:
```bash
npm run dev
```

### Mobile Setup

1. Install dependencies:
```bash
cd mobile
npm install
```

2. Set up environment variables:
Create a `.env` file in the mobile directory with:
```
API_URL=http://localhost:8000
FIREBASE_CONFIG=your_firebase_config
```

3. Start the Expo development server:
```bash
npx expo start
```

## API Documentation

The API documentation is available at `http://localhost:8000/docs` when the backend server is running.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 