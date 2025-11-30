# ZedPass

A modern, secure SSTP VPN client for Android built with Flutter and Material Design 3.

![Android](https://img.shields.io/badge/Android-8.0+-green.svg)
![Flutter](https://img.shields.io/badge/Flutter-3.x-blue.svg)

Telegram Channel: @CluvexStudio

## Features

- **SSTP VPN Protocol** - Secure Socket Tunneling Protocol support
- **Material Design 3** - Modern UI with Material You theming
- **Connection Management** - Easy connect/disconnect with status monitoring
- **Real-time Statistics** - Download/upload speed and total traffic tracking
- **Custom DNS** - Configure custom DNS servers
- **Proxy Support** - HTTP proxy configuration
- **SSL/TLS Options** - Configurable SSL versions (TLSv1, TLSv1.1, TLSv1.2, TLSv1.3)
- **Certificate Verification** - Optional hostname and SSL certificate verification
- **Persistent Settings** - Server configurations saved locally


## Requirements

- Android 8.0 (API 26) or higher
- Target SDK: Android 16 (API 36)

## Installation

### From Releases

1. Go to the [Releases](https://github.com/CluvexStudio/ZedPass/releases) page
2. Download the latest APK for your architecture:
   - `ZedPass-x.x.x-arm64-v8a.apk` - For modern 64-bit devices (recommended)
   - `ZedPass-x.x.x-armeabi-v7a.apk` - For older 32-bit devices
3. Install the APK on your Android device

### Build from Source

```bash
# Clone the repository
git clone https://github.com/CluvexStudio/ZedPass.git
cd ZedPass

# Install dependencies
flutter pub get

# Generate app icons
dart run flutter_launcher_icons

# Build release APK (arm64)
flutter build apk --target-platform android-arm64

# Build release APK (arm v7a)
flutter build apk --target-platform android-arm
```

The APK will be available at `build/app/outputs/flutter-apk/app-release.apk`

## Usage

1. Launch ZedPass
2. Tap the settings icon to configure your VPN server
3. Enter your server details:
   - **Host** - VPN server address
   - **Port** - Server port (default: 443)
   - **Username** - Your VPN username
   - **Password** - Your VPN password
4. Optionally configure DNS, proxy, and advanced SSL settings
5. Save settings and tap the connect button

## Tech Stack

- **Flutter** - Cross-platform UI framework
- **Provider** - State management
- **sstp_flutter** - SSTP VPN protocol implementation
- **shared_preferences** - Local storage for settings

## Project Structure

```
lib/
├── main.dart              # App entry point
├── providers/
│   └── vpn_provider.dart  # VPN state management
├── screens/
│   ├── home_screen.dart   # Main connection screen
│   └── settings_screen.dart # Server configuration
└── theme/
    └── app_theme.dart     # Material Design 3 theme
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- [sstp_flutter](https://pub.dev/packages/sstp_flutter) - SSTP VPN Flutter plugin
- [Material Design 3](https://m3.material.io/) - Design system

## Support

If you find this project helpful, consider supporting the development:

**TRX (Tron):**
```
TRxVSHcoADZnBfztFmFb2TQopusAwWYEVR
```

**BTC (Bitcoin):**
```
bc1qnjnvzsa5avgj7n0uy383cv5zdxfjnvvp257egm
```

**XRP (Ripple):**
```
rHnZrb5o2bi9sHsbux5e3vtraaPtZ32WQF
```

Thank you for your support! 🚀
