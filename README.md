# Stonk AI - AI-Powered Stock Analysis

An intelligent stock market analysis and prediction platform that leverages AI to analyze financial data, news, and market trends for informed investment decisions.

## Features

- 🔍 **Stock Search** - Detailed stock information and analysis
- 🤖 **AI Sentiment Analysis** - News headline sentiment analysis
- 🔮 **Price Predictions** - AI-powered future price predictions
- 📰 **News Integration** - Latest financial news aggregation
- 📹 **Video Analysis** - YouTube video content analysis
- 📊 **Options Data** - Options chain and analysis
- 🎨 **Custom Themes** - Dark/light theme support
- 📈 **Market Analysis** - Fear and greed indicators
- 👥 **User Features** - Authentication and user posts (planned)
- 💼 **Portfolio Tracking** - Personal investment tracking (planned)

## Tech Stack

- **Frontend**: React with Vite, TypeScript, TailwindCSS
- **Backend**: Python FastAPI with async support
- **AI Integration**: OpenAI GPT models for analysis
- **Data Sources**: Multiple financial APIs and news sources
- **Database**: SQLite for development, PostgreSQL for production
- **Deployment**: Docker containerization support

## Prerequisites

### Client
- Node.js (v16 or higher)
- npm or yarn or pnpm
- YouTube API key (for video analysis)
- OpenAI API key (for AI features)

### Server
- Python 3.8+
- FastAPI and Uvicorn
- Various financial data APIs (configurable)

## Environment Variables

### Client (.env)
```env
VITE_YOUTUBE_API_KEY=your_youtube_api_key
VITE_OPENAI_API_KEY=your_openai_api_key
VITE_SERVER_URL=http://localhost:8000
```

### Server (.env)
```env
# API Keys for various financial data sources
# Database configuration
# OpenAI configuration
```

## Getting Started

### Client Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd stonk-ai/client
```

2. Install dependencies:
```bash
pnpm install
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your API keys
```

4. Start the development server:
```bash
pnpm run dev
```

5. Open your browser and navigate to `http://localhost:5173`

## Deployment

### Client
```bash
cd client
pnpm run build
```

### Server
```bash
cd server
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python main.py
```

### Production Deployment

- **Client**: Deploy to Vercel, Netlify, or any static hosting platform
- **Server**: Deploy to VPS, Railway, Render, or similar Python hosting
- **Database**: Use PostgreSQL for production data persistence

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests to improve the application.

## License

MIT License
