<div align="center">

# FinderClip

![256.png](https://i.imgant.com/v2/ftvuj3C.png)  
<img src="https://img.shields.io/badge/macOS-12.0+-blue.svg" alt="macOS">
<img src="https://img.shields.io/badge/Swift-5.9-orange.svg" alt="Swift">
<img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License">

**Intuitive Cut & Paste Experience for macOS Finder**

English | [简体中文](README.md)

</div>

---

## ✨ Introduction

FinderClip is a lightweight macOS menu bar app that brings the familiar **⌘X** and **⌘V** shortcuts to Finder for cutting and moving files, just like in Windows.

## 🎯 Features

| Feature | Description |
|---------|-------------|
| ✂️ **True Cut** | Use ⌘X to cut files in Finder |
| 📋 **Smart Paste** | Use ⌘V to move files to destination |
| 🎯 **Context Detection** | Auto-detect file selection vs text editing |
| 🔔 **Visual Feedback** | Clear notifications for cut/paste operations |
| ⏱️ **Timeout Protection** | Customizable timeout (1-30 minutes) |
| ⌨️ **Quick Cancel** | Press Esc to cancel cut operation |
| 🌐 **Bilingual Support** | Support Chinese/English language switching |
| 🚀 **Launch at Login** | Support for auto-start on boot |
| ⚙️ **Settings Panel** | Beautiful preferences interface |
| 🔄 **Auto Update** | Built-in Sparkle auto-update |

## 📖 Usage

### Basic Operations

```
1. ⌘X  - Select files in Finder and press ⌘X to cut
2. ⌘V  - Navigate to destination and press ⌘V to move
3. Esc - Press Esc to cancel cut state
```

## 🚀 Quick Start

### Requirements

- macOS 12.0 or later
- Xcode Command Line Tools

### Build from Source

**Option 1: Using Xcode (Recommended)**
```bash
git clone https://github.com/Wcowin/Mac-Finder-Clipboard.git
cd Mac-Finder-Clipboard
open FinderClip.xcodeproj
# Press ⌘R in Xcode to run
```

**Option 2: Command Line**
```bash
git clone https://github.com/Wcowin/Mac-Finder-Clipboard.git
cd Mac-Finder-Clipboard

# Build and run
./scripts/build.sh --run

# Or just build
./scripts/build.sh
```

### First Time Setup

1. After running, a scissors icon ✂️ will appear in the menu bar
2. If it shows "⚠ Click to grant permission...", click to open System Settings
3. Find and check FinderClip in the Accessibility list
4. Return to the app, menu bar shows "✓ Ready" - you're all set!

## 🛠 Technical Implementation

### Core Technologies

- **CGEvent API** - Intercept global keyboard events
- **Accessibility API** - Detect focused element state
- **UserNotifications** - Modern notification system
- **ServiceManagement** - Launch at login support

### How It Works

```
User presses ⌘X
    ↓
Check if in Finder
    ↓
Check if in text editing mode
    ↓
Simulate ⌘C to copy files
    ↓
Mark cut mode
    ↓
User presses ⌘V
    ↓
Convert to ⌘⌥V (system cut & paste)
    ↓
Files moved
```

## 📁 Project Structure

```
Mac-Finder-Clipboard/
├── main.swift                    # App entry point
├── AppDelegate.swift             # App delegate and menu bar
├── FinderCutPasteManager.swift   # Core functionality
├── SettingsManager.swift         # Settings management
├── SettingsWindowController.swift # Settings UI
├── Assets.xcassets/              # App icon assets
├── FinderClip.xcodeproj/         # Xcode project
├── Info.plist                    # App configuration
├── FinderClip.entitlements       # Permissions
├── appcast.xml                   # Sparkle update feed
├── build.sh                      # Build script entry
├── scripts/
│   └── build.sh                  # Full build/release script
├── tools/sparkle/                # Sparkle signing tools
├── LICENSE                       # MIT License
└── README.md                     # Documentation
```

## 🚀 Build Commands

```bash
./scripts/build.sh              # Build Debug version
./scripts/build.sh --run        # Build and run
./scripts/build.sh --release    # Build Release version
./scripts/build.sh --release 1.0.4  # Release v1.0.4
./scripts/build.sh --clean      # Clean build files
./scripts/build.sh --status     # Show project status
./scripts/build.sh --help       # Show help
```

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Feel free to open an [Issue](https://github.com/Wcowin/Mac-Finder-Clipboard/issues) to report bugs or suggest new features!

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 👨‍💻 Author

**Wcowin** - [GitHub](https://github.com/Wcowin)

## ⭐ Star History

If this project helps you, please give it a Star ⭐

---

<div align="center">
  Made with ❤️ by Wcowin
</div>
