# ☁️ Cloudy - Flutter Login App

A modern and beautiful Flutter login application with API authentication integration.

![Flutter](https://img.shields.io/badge/Flutter-3.11.1-blue?logo=flutter)
![Dart](https://img.shields.io/badge/Dart-3.11.1-blue?logo=dart)
![License](https://img.shields.io/badge/license-MIT-green)

## 📱 Features

- ✨ **Beautiful UI Design** - Modern gradient design with smooth animations
- 🔐 **API Authentication** - Secure login with token-based authentication
- 🎨 **Google Fonts Integration** - Elegant typography using Poppins font
- 🔄 **Navigation System** - Clean routing between login and home pages
- 📱 **Multi-Platform Support** - Works on Android, iOS, Web, Windows, macOS, and Linux
- 🚀 **HTTP Integration** - RESTful API communication using http package

## 🖼️ Screenshots

<div align="center">
  <img src="screenshots/login.png" alt="Login Screen" width="200"/>
  <img src="screenshots/home.png" alt="Home Screen" width="200"/>
</div>

## 🚀 Getting Started

### Prerequisites

- Flutter SDK (>=3.11.1)
- Dart SDK (>=3.11.1)
- A running backend API server for authentication

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/cloudy.git
   cd cloudy
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Configure the API endpoint**
   
   Update the `baseUrl` in `lib/login_page.dart`:
   ```dart
   final String baseUrl = "http://your-api-server.com/api/login";
   ```

4. **Run the app**
   ```bash
   flutter run
   ```

## 📁 Project Structure

```
cloudy/
├── lib/
│   ├── main.dart          # App entry point & routing configuration
│   ├── login_page.dart    # Login screen with authentication logic
│   └── home_page.dart     # Dashboard/home screen after login
├── test/                  # Test files
├── pubspec.yaml           # Project dependencies & configuration
└── README.md              # Project documentation
```

## 🛠️ Dependencies

| Package | Version | Description |
|---------|---------|-------------|
| `flutter` | SDK | UI framework |
| `http` | ^1.6.0 | HTTP client for API calls |
| `google_fonts` | ^8.0.2 | Custom fonts for beautiful typography |
| `cupertino_icons` | ^1.0.8 | iOS-style icons |

## 🔌 API Requirements

Your backend API should support the following endpoint:

### Login Endpoint
```
POST /api/login
Content-Type: application/x-www-form-urlencoded

Parameters:
- email: string
- password: string

Response (200 OK):
{
  "token": "your-auth-token-here"
}
```

## 🎨 Customization

### Change Theme Colors
Edit the gradient colors in `lib/login_page.dart`:
```dart
LinearGradient(
  begin: Alignment.topCenter,
  colors: [Colors.blue[900]!, Colors.blue[800]!, Colors.blue[400]!],
)
```

### Modify Routes
Update routes in `lib/main.dart`:
```dart
routes: {
  '/login': (context) => Login(),
  '/home': (context) => HomePage(),
},
```

## 🧪 Testing

Run tests with:
```bash
flutter test
```

## 📦 Building for Production

### Android
```bash
flutter build apk --release
# or
flutter build appbundle --release
```

### iOS
```bash
flutter build ios --release
```

### Web
```bash
flutter build web --release
```

### Windows
```bash
flutter build windows --release
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- Email: your.email@example.com

## 🙏 Acknowledgments

- [Flutter](https://flutter.dev/) - Amazing UI framework
- [Google Fonts](https://fonts.google.com/) - Beautiful typography
- [HTTP package](https://pub.dev/packages/http) - HTTP client library

---

<div align="center">

**Made with ❤️ using Flutter**

If you like this project, please give it a ⭐️!

</div>
