# ☕ Coffee Shop UI

A beautiful, modern cross-platform coffee shop application built with Flutter. Browse, filter, and discover your favorite coffee varieties with an elegant user interface designed for the perfect coffee experience.

![Flutter](https://img.shields.io/badge/Flutter-3.5%2B-blue?style=flat-square&logo=flutter)
![Dart](https://img.shields.io/badge/Dart-3.5%2B-0175C2?style=flat-square&logo=dart)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20Android%20%7C%20Windows%20%7C%20macOS%20%7C%20Linux-black?style=flat-square)

---

## ✨ Features

🎨 **Modern Dark Theme UI**
- Sleek dark interface with orange accent colors
- Smooth animations and intuitive navigation
- Responsive design that adapts to all screen sizes

🔍 **Smart Search & Filtering**
- Real-time coffee search functionality
- Filter by coffee types (Cappuccino, Latte, Black, etc.)
- Quick category switching

☕ **Coffee Catalog**
- Browse premium coffee varieties
- View detailed pricing
- Professional coffee imagery
- Add to favorites

📱 **Cross-Platform Support**
- iOS & Android
- Windows & macOS
- Linux
- Write once, run everywhere

🧭 **Intuitive Navigation**
- Bottom navigation bar
- Home, Favorites, and Notifications tabs
- User profile quick access
- Menu drawer

🎯 **User-Centric Design**
- Material Design principles
- Accessibility-first approach
- Fast and lightweight performance
- Smooth user experience

---

## 🚀 Quick Start

### Prerequisites

Before you begin, ensure you have the following installed:

- **Flutter SDK** (v3.5.3 or higher) - [Install Flutter](https://flutter.dev/docs/get-started/install)
- **Dart SDK** (comes with Flutter)
- **Git**
- Platform-specific requirements:
  - **iOS**: Xcode (macOS only)
  - **Android**: Android Studio or Android SDK
  - **Windows**: Visual Studio Build Tools
  - **macOS**: Xcode
  - **Linux**: CMake, GTK development files

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/chahmadraza89/Coffee-Shop-Ui.git
   cd Coffee-Shop-Ui/flutter_app
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   flutter run
   ```

---

## 📦 Build & Run

### Run in Development Mode

```bash
# Run on connected device/emulator
flutter run

# Run on specific device
flutter run -d <device_id>

# List available devices
flutter devices
```

### Build for Production

**Android**
```bash
flutter build apk --release
flutter build appbundle --release
```

**iOS**
```bash
flutter build ios --release
```

**Windows**
```bash
flutter build windows --release
```

**macOS**
```bash
flutter build macos --release
```

**Linux**
```bash
flutter build linux --release
```

---

## 📂 Project Structure

```
flutter_app/
├── lib/
│   ├── main.dart                 # Application entry point
│   ├── pages/
│   │   ├── home_pages.dart       # Home screen with coffee catalog
│   │   ├── coffeetypes.dart      # Coffee type filter widget
│   │   └── utill/
│   │       └── coffee_tiles.dart # Individual coffee tile component
│   └── assets/
│       └── images/               # Coffee images (cappuccino, latte, etc.)
├── android/                      # Android-specific code
├── ios/                          # iOS-specific code
├── windows/                      # Windows-specific code
├── macos/                        # macOS-specific code
├── linux/                        # Linux-specific code
├── pubspec.yaml                  # Project dependencies
└── analysis_options.yaml         # Dart linting rules
```

### Key Files Description

| File | Purpose |
|------|---------|
| `main.dart` | App initialization and theme configuration (dark theme with orange accent) |
| `home_pages.dart` | Main UI with search bar, coffee filters, and product grid |
| `coffee_tiles.dart` | Reusable coffee product card component |
| `pubspec.yaml` | Project configuration and dependencies (Flutter, Cupertino Icons, Google Fonts) |

---

## 🛠️ Tech Stack

- **Framework**: [Flutter](https://flutter.dev/) - Cross-platform UI toolkit
- **Language**: [Dart](https://dart.dev/) - Modern programming language
- **UI Components**: 
  - Material Design
  - Cupertino Icons
  - Google Fonts (Bebas Neue)
- **Build System**: CMake (Windows, Linux, macOS)
- **State Management**: setState (StatefulWidget)
- **Package Manager**: Pub

---

## 🎯 Core Features Breakdown

### Home Screen (`home_pages.dart`)
- Welcome headline: "Find the best coffee for you"
- Search bar with live filtering
- Horizontal scrollable coffee type selector
- Horizontal scrollable coffee product grid
- Bottom navigation for Home, Favorites, and Notifications

### Coffee Types Filter
- Cappuccino (default selected)
- Latte
- Black
- Expandable for additional types

### Coffee Catalog
- Product name
- Product image
- Price display
- Smooth horizontal scrolling

---

## 🎨 Customization

### Change Theme Colors

Edit `main.dart`:
```dart
theme: ThemeData(
  brightness: Brightness.dark,
  primarySwatch: Colors.orange,  // Change this color
),
```

### Add New Coffee Types

Edit `home_pages.dart`:
```dart
final List coffeeTypes = [
  ["Cappuccino", true],
  ["Latte", false],
  ["Black", false],
  ["Espresso", false],  // Add new type here
];
```

### Add New Coffee Products

Edit `home_pages.dart` in the ListView builder:
```dart
CoffeeTiles(
  coffeeImagePath: "assets/images/your_image.jpg",
  coffeeName: "Coffee Name",
  coffeePrice: "4.50",
),
```

---

## 📋 Dependencies

```yaml
flutter: ^3.5.3
cupertino_icons: ^1.0.8
google_fonts: ^latest
flutter_lints: ^4.0.0
```

To update dependencies:
```bash
flutter pub upgrade
```

---

## 🔮 Future Enhancements

- [ ] User authentication & profiles
- [ ] Shopping cart functionality
- [ ] Order history
- [ ] Payment integration (Stripe, PayPal)
- [ ] Real-time database (Firebase)
- [ ] Customer reviews & ratings
- [ ] Coffee brewing guides
- [ ] Loyalty program
- [ ] In-app notifications
- [ ] Dark/Light theme toggle

---

## 🤝 Contributing

Contributions are welcome! Here's how to contribute:

1. **Fork the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/Coffee-Shop-Ui.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```

3. **Commit your changes**
   ```bash
   git commit -m 'Add amazing feature'
   ```

4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```

5. **Open a Pull Request**

### Code Style Guidelines
- Follow Dart [style guide](https://dart.dev/guides/language/effective-dart/style)
- Use meaningful variable names
- Add comments for complex logic
- Run `flutter analyze` before committing

---

## 🐛 Troubleshooting

### Common Issues

**Flutter not found?**
```bash
flutter --version  # Verify installation
export PATH="$PATH:`pwd`/flutter/bin"  # Add to PATH
```

**Dependencies not loading?**
```bash
flutter clean
flutter pub get
```

**Build failures on specific platform?**
```bash
flutter clean
rm -rf build/
flutter pub get
flutter run
```

**Hot reload not working?**
- Try `flutter run` instead of using IDE
- Check if file was saved
- Try full app restart with `R`

---

## 📱 Screenshots & Demo

Experience the smooth UI with:
- Dark, elegant interface
- Instant coffee filtering
- Beautiful product cards
- Smooth scrolling and animations

Run the app to see it in action!

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Chahmad Raza**

- GitHub: [@chahmadraza89](https://github.com/chahmadraza89)
- Repository: [Coffee-Shop-Ui](https://github.com/chahmadraza89/Coffee-Shop-Ui)

---

## 📞 Support & Feedback

Have questions or suggestions? 

- Open an [Issue](https://github.com/chahmadraza89/Coffee-Shop-Ui/issues)
- Create a [Discussion](https://github.com/chahmadraza89/Coffee-Shop-Ui/discussions)
- Check existing [Issues](https://github.com/chahmadraza89/Coffee-Shop-Ui/issues?q=is%3Aissue)

---

## 🙏 Acknowledgments

- Flutter team for the amazing framework
- Material Design for design guidelines
- Community for inspiration and feedback

---

<div align="center">

**⭐ If you like this project, please consider giving it a star!**

Made with ☕ and ❤️ by Chahmad Raza

</div>
