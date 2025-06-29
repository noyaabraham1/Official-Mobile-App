# Besmi Mobile App

Professional lash booking platform mobile application built with Capacitor.

## Description

Besmi is a comprehensive lash booking and business management platform designed for lash artists. This mobile app provides direct access to the full Besmi platform at https://besmi.replit.app.

## Features

- Professional lash artist booking system
- Client management and scheduling
- Payment processing integration
- Appointment notifications
- Business analytics and insights
- Native mobile experience with splash screen
- Camera access for profile photos
- Push notifications support
- Haptic feedback

## Build Instructions

This repository uses GitHub Actions to automatically build Android APK files.

### Building APK

1. Go to the "Actions" tab in this repository
2. Select "Build Android APK" workflow
3. Click "Run workflow" button
4. Wait for completion (10-15 minutes)
5. Download APK from artifacts section

### Manual Build

If you prefer building locally with Android Studio:

1. Clone this repository
2. Install dependencies: `npm install`
3. Sync Capacitor: `npx cap sync`
4. Open in Android Studio: `npx cap open android`
5. Build > Generate Signed Bundle/APK

## Technical Details

- **Platform**: Capacitor (Cross-platform mobile framework)
- **Target**: Android 7.0+ devices
- **Backend**: Connects to https://besmi.replit.app
- **Build System**: GitHub Actions + Gradle
- **Package ID**: com.besmi.lashbooking

## App Architecture

The mobile app uses a hybrid approach:
- Native Android shell with Capacitor plugins
- WebView displaying the live web platform
- Automatic updates without app store resubmission
- Native features: camera, notifications, haptics

## Installation

The generated APK can be:
- Installed directly on Android devices (enable "Install from unknown sources")
- Submitted to Google Play Store for distribution
- Distributed via internal testing channels

## Development

This app wraps the existing Besmi web platform, providing:
- Native mobile experience
- Offline capabilities
- Push notifications
- Device integration (camera, contacts, etc.)

## License

MIT License