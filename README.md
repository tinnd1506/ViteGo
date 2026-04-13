# ViteGo - Modern Ride Sharing Platform

ViteGo is a full-stack ride-sharing application built with Flask, featuring a modern glassmorphism UI, real-time chat, and seamless payment processing.

🌐 **Live Demo**: https://vitego.onrender.com/

📁 **GitHub**: https://github.com/tinnd1506/ViteGo/tree/main



## ✨ Features

### Modern UI/UX
- **Glassmorphism Design**: Frosted glass effects with backdrop blur
- **Responsive Layout**: Mobile-friendly interface
- **Smooth Animations**: CSS transitions and hover effects
- **3D Car Showcase**: Interactive vehicle selection with pricing

### User Features
- **Easy Booking**: Pick-up & drop-off location selection with Google Maps
- **Car Options**: ViteGo, ViteGo XL with dynamic pricing
- **Time Scheduling**: Schedule rides with custom pickup times
- **Real-time Chat**: Live messaging with drivers via Socket.IO
- **Payment Integration**: Secure payment processing with email confirmation
- **Ride History**: View past rides and receipts

### Driver Features
- **Dashboard**: View available ride requests with earnings tracking
- **Map Integration**: View passenger pickup locations
- **Ride Acceptance**: One-click ride confirmation
- **Earnings Tracker**: Lifetime earnings and completed rides history
- **Real-time Chat**: Communicate with passengers

## �️ Tech Stack

- **Backend**: Flask 3.0 (Python 3.10+)
- **Database**: SQLite (users), MongoDB Atlas (rides, chat)
- **Real-time**: Flask-SocketIO
- **Maps**: Google Maps API (Places, Distance Matrix, Directions)
- **Email**: Brevo API (transactional emails)
- **Frontend**: HTML5, CSS3 (Glassmorphism), JavaScript, jQuery

## 🚀 Getting Started

### Prerequisites
- Python 3.10+
- Google Maps API key
- MongoDB Atlas cluster
- Brevo account (for email receipts)

### Installation

1. **Clone the repo**
   ```bash
   git clone https://github.com/tinnd1506/ViteGo.git
   cd ViteGo
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   ```bash
   copy .env.example .env
   ```
   Edit `.env` with your actual values (see below).

4. **Run the app**
   ```bash
   python run.py
   ```

5. **Open** http://localhost:5000

### Environment Variables

| Variable | Description | Example |
|---|---|---|
| `SECRET_KEY` | Flask session secret | `your-secret-key` |
| `GOOGLE_MAPS_API_KEY` | Google Maps API key | `AIzaSy...` |
| `MONGO_DB_URL` | MongoDB connection string | `mongodb+srv://...` |
| `MONGO_DB_NAME` | MongoDB database name | `uber_clone` |
| `SQLITE_DB_NAME` | SQLite database file | `database.db` |
| `BREVO_API_KEY` | Brevo API key for emails | `xkeysib-...` |
| `MAIL_DEFAULT_SENDER` | Verified sender email | `your@email.com` |

### Setting up Brevo (Email)

1. Create a free account at [brevo.com](https://www.brevo.com)
2. Go to **Settings → SMTP & API → API Keys** → create a key
3. Go to **Settings → Senders & IP** → add and verify your sender email
4. Add `BREVO_API_KEY` and `MAIL_DEFAULT_SENDER` to your `.env`

> **Note**: SMTP ports (25, 465, 587) are blocked on Render's free tier. Brevo's HTTP API bypasses this restriction.

## �� User Guide

### For Passengers
1. Visit https://vitego.onrender.com/ and click "Ride Now"
2. Register/Login as User
3. Enter pickup & destination locations
4. Select preferred car type (ViteGo, ViteGo XL)
5. Choose pickup time (default: now + 5 min)
6. Confirm ride → Chat with driver
7. Complete payment → Get email receipt
8. View ride history anytime

### For Drivers
1. Visit https://vitego.onrender.com/ and click "Drive With Us"
2. Register/Login as Driver

## 🔧 Troubleshooting

### Common Issues

1. **Flask 3.0 Compatibility**: All extensions updated to latest versions
2. **MongoDB Connection**: Ensure IP whitelist includes Render's outbound IPs
3. **Google Maps API**: Enable Places, Distance Matrix, and Geocoding APIs
4. **Email Sending**: Uses Brevo API (SMTP ports are blocked on Render free tier)

### Render Deployment
- Free tier: Sleeps after 15 min inactivity (use UptimeRobot to keep alive)
- Environment variables set in Render Dashboard
- Auto-deploys on git push to main branch

## 📝 License

MIT License - Feel free to use and modify!

## 🤝 Contributing

Pull requests welcome! For major changes, please open an issue first.

## 🙏 Acknowledgments

- Google Maps Platform for location services
- MongoDB Atlas for database hosting
- Render for free deployment hosting
- Brevo for transactional email API
- Flask community for excellent web framework

---

**Built with ❤️ using Flask & Modern CSS**
