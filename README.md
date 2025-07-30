# Virtual Membership Card - Flutter App

A sleek and modern Flutter application that displays a virtual membership card with dynamically generated QR codes. Perfect for businesses that need to provide digital membership cards to their customers.

## 🌟 Features

- **Beautiful UI Design**: Modern gradient card design with smooth animations
- **Dynamic QR Code Generation**: QR codes are generated in real-time based on user data
- **Time-Sensitive Tokens**: QR codes can be refreshed with timestamp-based tokens
- **Responsive Design**: Optimized for various screen sizes
- **Smooth Animations**: Fade transitions and visual feedback for better UX

## 📱 Screenshots

### Main Screen
The app displays a premium-looking membership card with:
- User profile section (Alex Ray - Platinum Member)
- Circular profile picture placeholder
- Dynamically generated QR code in the center
- Card ID display
- Refresh button for generating new QR codes

### Key UI Elements
- **Gradient Background**: Beautiful purple-blue gradient card design
- **Profile Section**: Displays user name and membership level
- **QR Code Area**: Clean white background with centered QR code
- **Interactive Button**: Prominent refresh button with icon
- **Status Feedback**: Success message when QR code is refreshed

## 🛠️ Tech Stack

- **Flutter**: Cross-platform mobile development framework
- **qr_flutter**: Library for QR code generation
- **Material Design**: Modern UI components and animations

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (3.0.0 or higher)
- Dart SDK
- Android Studio / VS Code
- iOS Simulator / Android Emulator

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Priyanka1823/virtual-membership-card.git
   cd virtual-membership-card
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   flutter run
   ```

## 📋 Project Structure

```
lib/
├── constants/
│ ├── colors.dart
│ ├── dimensions.dart
│ └── text_styles.dart
├── screen/
│ └── membership_card_screen.dart
├── utils/
│ └── app_utils.dart
├── widgets/
│ ├── membership_card.dart
│ └── refresh_button.dart
└── main.dart
```

## 🔧 Key Implementation Details

### QR Code Generation
- Base user ID: `"user-id-12345-abcde"`
- Dynamic QR data format: `"user-id-12345-abcde-{timestamp}"`
- Uses `qr_flutter` package for reliable QR code rendering

### State Management
- Uses Flutter's built-in `StatefulWidget` and `setState()`
- Manages QR code data updates efficiently
- Handles animation states for smooth transitions

### UI Components
- **Custom Card Design**: Gradient background with rounded corners
- **Profile Section**: Icon placeholder and user information
- **QR Code Container**: White background with shadow effects
- **Interactive Button**: Material Design elevated button with icon

## 🎯 Core Functionality

### QR Code Refresh Feature
When the "Refresh QR Code" button is pressed:
1. Current timestamp is appended to base user ID
2. QR code is regenerated with new data
3. Fade animation plays for smooth transition
4. Success snackbar appears to confirm action
5. Card ID display updates to show new identifier

### Demo
![Screen Recording 2025-07-30 124512](https://github.com/user-attachments/assets/ca0f1a39-5808-404e-97db-f9e407364a8d)

### Screenshots 
<img width="360" height="764" alt="Screenshot 2025-07-30 124430" src="https://github.com/user-attachments/assets/808a35c9-f500-43dd-a7df-eb842b3ad303" />

**base Scanner output**
![WhatsApp Image 2025-07-30 at 16 26 49_c225e624](https://github.com/user-attachments/assets/d122b1c4-d4f7-46e4-9257-93b22a395a6e)

**After Refreshing Scanner Output**
![WhatsApp Image 2025-07-30 at 16 26 48_41c5e31c](https://github.com/user-attachments/assets/ddfa27f4-0e49-4828-a261-3504852b7634)



### Example QR Data Flow
- **Initial**: `user-id-12345-abcde`
- **After Refresh**: `user-id-12345-abcde-1699123456789`
- **Next Refresh**: `user-id-12345-abcde-1699123467890`

## 📦 Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter
  qr_flutter:     # QR code generation
  cupertino_icons:    # iOS-style icons
```

## 🎨 Design Features

- **Modern Gradient**: Purple to blue gradient background
- **Card Shadow**: Elevated card appearance with depth
- **Rounded Corners**: Consistent 20px border radius
- **White QR Background**: High contrast for better scanning
- **Typography**: Roboto font family for clean readability
- **Color Scheme**: Professional blue-gray theme


## 📱 Platform Support

- ✅ Android
- ✅ iOS
- 📋 Web (with limitations on QR scanning)

---


The QR code contains the user ID with a timestamp, making each code unique and time-sensitive - perfect for security-conscious applications.

---

**Built with ❤️ using Flutter**
