# CropGuard - Smart Farming Companion 🌱

A comprehensive Flutter web application designed to help farmers and gardeners identify plant diseases, share knowledge with the farming community, and receive weather-based farming advice.

![CropGuard Banner](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)

## 🚀 Features

### 🔍 Disease Detection
- **AI-Powered Analysis**: Upload plant photos for instant disease identification
- **Treatment Recommendations**: Get specific treatment plans for detected diseases
- **Prevention Tips**: Learn how to prevent future occurrences
- **Confidence Scoring**: AI provides confidence levels for accurate diagnosis

### 🌤️ Weather-Based Advice
- **Current Weather**: Real-time weather data for your location
- **5-Day Forecast**: Plan your farming activities in advance
- **Farming Recommendations**: Weather-specific advice for optimal crop care
- **Weather Alerts**: Important warnings for weather conditions affecting crops

### 👥 Community Features
- **Knowledge Sharing**: Share tips, problems, and success stories
- **Expert Advice**: Get help from experienced farmers and gardeners
- **Categorized Posts**: Tips, problems, questions, and success stories
- **Interactive Comments**: Engage with the community through likes and comments
- **Tagging System**: Find relevant content easily with hashtags

### 📱 User Profile & Tracking
- **Personal Dashboard**: Track your farming journey and achievements
- **Garden Journal**: Keep records of your plants and treatments
- **Achievement System**: Earn badges for community participation
- **Statistics**: Monitor your scanning history and community contributions

## 🛠️ Technologies

- **Frontend**: Flutter (Dart)
- **UI**: Material Design 3
- **State Management**: StatefulWidget (Provider/Riverpod ready)
- **Platform**: Web, Android, iOS, Windows, macOS, Linux
- **APIs**: Weather API integration, AI/ML service ready

## 📋 Prerequisites

- Flutter SDK (3.19.6 or higher)
- Dart SDK
- Web browser for testing
- IDE (VS Code recommended, Android Studio, or IntelliJ)

## ⚡ Quick Start

### Option 1: Automated Installation (Windows)

Run the provided installation script as Administrator:

```powershell
# PowerShell (Recommended)
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
.\install_flutter.ps1
```

Or use the batch file:
```cmd
install_flutter.bat
```

### Option 2: Manual Installation

1. **Install Flutter SDK**
   ```bash
   # Download Flutter SDK from https://docs.flutter.dev/get-started/install
   # Extract to C:\flutter (Windows) or appropriate directory
   # Add flutter/bin to your PATH
   ```

2. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/cropguard.git
   cd cropguard
   ```

3. **Install dependencies**
   ```bash
   flutter pub get
   ```

4. **Run the application**
   ```bash
   flutter run -d chrome
   ```

## 📁 Project Structure

```
lib/
├── main.dart              # App entry point with navigation
├── models/
│   └── app_models.dart    # Data models (User, Post, Weather, etc.)
├── screens/
│   ├── homescreen.dart    # Home dashboard
│   ├── disease_detection.dart # AI disease analysis
│   ├── community.dart     # Social platform features
│   ├── weather_advice.dart # Weather data & advice
│   └── profile.dart       # User profile & statistics
└── services/
    └── api_service.dart   # API integrations & HTTP requests
```

## 🔧 Configuration

### Weather API Setup
1. Sign up for [OpenWeatherMap API](https://openweathermap.org/api)
2. Replace `YOUR_API_KEY_HERE` in [`lib/services/api_service.dart`](lib/services/api_service.dart)
3. Configure location services as needed

### Disease Detection API
1. Set up your AI/ML service endpoint
2. Update the base URL in [`lib/services/api_service.dart`](lib/services/api_service.dart)
3. Implement authentication if required

## 📱 Screenshots

| Home Screen | Disease Detection | Community | Weather Advice |
|-------------|-------------------|-----------|----------------|
| ![Home](screenshots/home.png) | ![Detection](screenshots/detection.png) | ![Community](screenshots/community.png) | ![Weather](screenshots/weather.png) |

## 🚀 Build & Deploy

### Development
```bash
flutter run -d chrome
```

### Production Build
```bash
# Web
flutter build web

# Android
flutter build apk

# iOS
flutter build ios

# Windows
flutter build windows
```

## 📦 Dependencies

```yaml
dependencies:
  flutter: sdk: flutter
  http: ^1.1.0           # API requests
  image_picker: ^1.0.4   # Camera/gallery access
  shared_preferences: ^2.2.2  # Local storage
  intl: ^0.18.1          # Internationalization
```

## 🛣️ Roadmap

### Planned Features
- [ ] **Offline Mode**: Cache critical data for offline access
- [ ] **Push Notifications**: Weather alerts and community updates
- [ ] **Multi-language Support**: Localization for global users
- [ ] **Advanced Analytics**: Detailed farming insights and trends
- [ ] **Market Prices**: Real-time crop pricing information
- [ ] **Expert Consultations**: Direct access to agricultural experts

### Technical Improvements
- [ ] **State Management**: Implement Provider or Riverpod
- [ ] **Database Integration**: Local SQLite for offline data
- [ ] **Image Caching**: Optimize image loading and storage
- [ ] **Performance Optimization**: Lazy loading and code splitting

## 🤝 Contributing

We welcome contributions to CropGuard! Please feel free to submit issues, feature requests, or pull requests.

### Development Guidelines
1. Follow Flutter/Dart style guidelines
2. Write clear commit messages
3. Test your changes thoroughly
4. Update documentation as needed

### Getting Started with Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🐛 Troubleshooting

- **Flutter not found**: Restart VS Code after installation
- **Dependencies error**: Run `flutter clean && flutter pub get`
- **Build issues**: Check Flutter doctor with `flutter doctor`
- **Web issues**: Ensure Chrome is installed and updated

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Flutter team for the amazing framework
- Material Design for UI components
- OpenWeatherMap for weather data
- The farming community for inspiration and feedback

## 📞 Support

For support or questions about CropGuard:
- 📧 Email: support@cropguard.app
- 🐛 Issues: [GitHub Issues](https://github.com/yourusername/cropguard/issues)
- 💬 Discussions: [GitHub Discussions](https://github.com/yourusername/cropguard/discussions)

---

**CropGuard** - Empowering farmers with technology for better crop management and community collaboration. 🌱

[![Made with Flutter](https://img.shields.io/badge/Made%20with-Flutter-blue.svg)](https://flutter.dev/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
