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

## 📱 User Guide

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
4. **Email Sending**: Use App Password for Gmail SMTP

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
- Flask community for excellent web framework

---

**Built with ❤️ using Flask & Modern CSS**
