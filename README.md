# VNtrades.in - Automated BTCUSDT Options Trading Platform

A professional-grade automated trading platform for BTCUSDT options on Delta Exchange, featuring advanced strategy logic, real-time monitoring, and comprehensive risk management.

## 🚀 Features

### Frontend (React + TypeScript)
- **Modern Dashboard**: Real-time trading dashboard with live data
- **Options Chain Viewer**: Complete options chain with live pricing
- **Strategy Configuration**: Configurable trading parameters
- **Trade History**: Comprehensive trade logging and analysis
- **Mobile Responsive**: Optimized for all devices
- **Real-time Updates**: WebSocket integration for live data

### Backend (FastAPI + Python)
- **Delta Exchange Integration**: Direct API integration
- **Advanced Strategy Logic**: Multi-condition signal generation
- **Risk Management**: Configurable stop-loss and take-profit
- **Paper Trading**: Safe testing environment
- **Real-time WebSocket**: Live data streaming
- **Comprehensive Logging**: All trades and signals logged

### Trading Strategy
The platform only executes trades when ALL conditions are met:
- **Minimum 7% ROI Target**: Ensures profitable trades
- **9.5/10 Confidence Score**: High-probability setups only
- **Order Block/Fair Value Gap**: Technical analysis confirmation
- **SMT Divergence**: Smart Money Theory signals
- **Volume Spike**: 2x average volume confirmation
- **IV Skew**: Implied volatility analysis

## 🛠 Installation

### Quick Start (Development)

1. **Clone the repository**
```bash
git clone <repository-url>
cd vntrader-platform
```

2. **Install frontend dependencies**
```bash
npm install
```

3. **Install backend dependencies**
```bash
cd backend
pip install -r requirements.txt
```

4. **Configure environment**
```bash
cp backend/.env.example backend/.env
# Edit .env with your Delta Exchange API credentials
```

5. **Start development servers**
```bash
# Terminal 1: Backend
cd backend
python -m uvicorn main:app --reload --port 8000

# Terminal 2: Frontend
npm run dev
```

### Production Deployment

#### Option 1: Railway.app
[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https://github.com/your-repo/vntrader)

#### Option 2: Render.com
[![Deploy to Render](https://deploy.to.render.com/button.svg)](https://render.com/deploy?repo=https://github.com/your-repo/vntrader)

#### Option 3: Docker
```bash
# Build and run with Docker Compose
docker-compose up --build -d
```

## ⚙️ Configuration

### Delta Exchange API Setup
1. Create account at [Delta Exchange](https://delta.exchange)
2. Generate API keys in your account settings
3. Add keys to `backend/.env`:
```env
DELTA_API_KEY=your_api_key_here
DELTA_API_SECRET=your_api_secret_here
```

### Strategy Parameters
Configure via the web interface or backend API:
- **Min ROI**: Minimum return on investment (default: 7%)
- **Confidence Threshold**: Signal confidence requirement (default: 9.5/10)
- **Volume Spike**: Required volume multiplier (default: 2.0x)
- **IV Threshold**: Minimum implied volatility (default: 25%)
- **Position Size**: Dollar amount per trade (default: $1000)
- **Stop Loss**: Maximum loss percentage (default: 50%)
- **Take Profit**: Target profit percentage (default: 200%)

## 📊 Trading Logic

### Signal Generation
The platform continuously monitors:
1. **Price Action**: Order blocks and fair value gaps
2. **Market Structure**: Smart Money Theory divergences
3. **Volume**: Unusual volume spikes
4. **Volatility**: Implied volatility skews
5. **Technical**: Multiple timeframe confirmations

### Risk Management
- **Paper Mode**: Test strategies without real money
- **Position Limits**: Maximum concurrent positions
- **Stop Loss**: Automatic loss limiting
- **Take Profit**: Automated profit taking
- **Account Protection**: Balance preservation logic

## 🔔 Notifications

The platform supports:
- **Browser Push**: Real-time in-browser notifications
- **Trade Alerts**: Entry and exit notifications
- **Signal Alerts**: High-confidence signal notifications
- **System Alerts**: Bot status and error notifications

## 📈 Monitoring & Analytics

### Dashboard Features
- Real-time P&L tracking
- Win rate statistics
- Performance charts
- Account balance monitoring
- Trade history analysis

### Logging
All activities are logged:
- Trade executions
- Signal generations
- Strategy changes
- System events
- API interactions

## 🔒 Security

- **API Key Protection**: Secure environment variable storage
- **Input Validation**: All user inputs validated
- **Rate Limiting**: API call rate limiting
- **Error Handling**: Comprehensive error management
- **Audit Trail**: Complete activity logging

## ⚠️ Important Disclaimers

1. **Financial Risk**: Trading involves substantial risk of loss
2. **No Guarantees**: Past performance doesn't guarantee future results
3. **Testing Required**: Thoroughly test strategies in paper mode
4. **Market Risk**: Cryptocurrency markets are highly volatile
5. **Technical Risk**: Software may contain bugs or errors

## 🤝 Support

### Documentation
- [API Documentation](./docs/api.md)
- [Strategy Guide](./docs/strategy.md)
- [Deployment Guide](./docs/deployment.md)

### Community
- [Discord Server](https://discord.gg/vntrader)
- [Telegram Group](https://t.me/vntrader)
- [GitHub Issues](https://github.com/your-repo/vntrader/issues)

## 📝 License

This software is provided for educational purposes. Users are responsible for compliance with local regulations and risk management.

## 🔄 Updates

The platform receives regular updates:
- Security patches
- Performance improvements
- New features
- Strategy enhancements

---

**Made with ❤️ for the trading community**

*Remember: Only trade with money you can afford to lose.*