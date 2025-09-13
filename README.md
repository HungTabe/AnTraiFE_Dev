# 🐔 AnTrai Android App - Smart Poultry Management

<div align="center">

![AnTrai Android](https://img.shields.io/badge/AnTrai-Android%20App-green?style=for-the-badge&logo=android)

**Ứng dụng Android quản lý đàn gia cầm thông minh với AI Assistant**

[![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=flat&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=flat&logo=android&logoColor=white)](https://developer.android.com/)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat&logo=jetpack-compose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![Material Design](https://img.shields.io/badge/Material%20Design-757575?style=flat&logo=material-design&logoColor=white)](https://material.io/)

</div>

---

## 📋 Tổng quan dự án

**AnTrai Android App** là ứng dụng di động được phát triển bằng Kotlin, cung cấp giao diện người dùng trực quan và thân thiện cho hệ thống quản lý đàn gia cầm thông minh. Ứng dụng tích hợp đầy đủ các tính năng từ backend API và tối ưu hóa cho trải nghiệm di động.

### 🎯 Mục tiêu chính
- **Giao diện di động** trực quan và dễ sử dụng
- **Đồng bộ real-time** với backend server
- **AI Assistant** tích hợp chat bot thông minh
- **Quản lý offline** với khả năng sync khi có mạng
- **Thông báo push** cho các sự kiện quan trọng
- **Tối ưu hiệu năng** cho thiết bị Android

---

## 🏗️ Kiến trúc ứng dụng

### Android App Structure
```
app/
├── src/main/
│   ├── java/com/antrai/
│   │   ├── ui/                    # UI Components & Screens
│   │   │   ├── auth/              # Authentication Screens
│   │   │   ├── poultry/           # Poultry Management
│   │   │   ├── care/              # Health & Care
│   │   │   ├── ai/                # AI Assistant
│   │   │   ├── expert/            # Expert Consultation
│   │   │   ├── reports/           # Reports & Analytics
│   │   │   └── profile/           # User Profile
│   │   ├── data/                  # Data Layer
│   │   │   ├── api/               # API Services
│   │   │   ├── local/             # Local Database (Room)
│   │   │   ├── repository/        # Repository Pattern
│   │   │   └── model/             # Data Models
│   │   ├── domain/                # Business Logic
│   │   │   ├── usecase/           # Use Cases
│   │   │   ├── repository/        # Repository Interfaces
│   │   │   └── model/             # Domain Models
│   │   ├── di/                    # Dependency Injection
│   │   ├── utils/                 # Utility Functions
│   │   └── MainActivity.kt        # Main Activity
│   ├── res/                       # Resources
│   │   ├── layout/                # XML Layouts (if needed)
│   │   ├── values/                # Strings, Colors, Styles
│   │   ├── drawable/              # Icons & Images
│   │   └── mipmap/                # App Icons
│   └── AndroidManifest.xml        # App Manifest
├── build.gradle.kts               # App-level build config
└── proguard-rules.pro             # ProGuard rules
```

### Architecture Pattern
- **MVVM (Model-View-ViewModel)** với Jetpack Compose
- **Repository Pattern** cho data management
- **Dependency Injection** với Hilt
- **Reactive Programming** với Kotlin Coroutines & Flow
- **Offline-First** approach với Room database

---

## 🚀 Tính năng chính

### 🔐 Authentication & User Management
- [x] Đăng nhập/Đăng ký với JWT
- [x] Remember me & Auto-login
- [x] Profile management
- [x] Role-based UI (Farmer/Expert/Admin)
- [x] Secure token storage

### 🐔 Poultry Management
- [x] Danh sách đàn gia cầm với search & filter
- [x] Thêm/sửa/xóa thông tin gia cầm
- [x] Upload ảnh từ camera/gallery
- [x] Chi tiết thông tin từng con
- [x] Phân loại theo giống, tuổi, sức khỏe
- [x] Quản lý chuồng trại

### 🏥 Health & Care Management
- [x] Dashboard sức khỏe tổng quan
- [x] Lịch chăm sóc và tiêm phòng
- [x] Ghi chép hoạt động chăm sóc
- [x] Lịch sử y tế và điều trị
- [x] Cảnh báo và nhắc nhở
- [x] Health tracking charts
- [x] Medication reminders

### 🤖 AI Assistant
- [x] Chat interface với AI
- [x] Chẩn đoán triệu chứng qua ảnh
- [x] Tư vấn kỹ thuật chăn nuôi
- [x] Cơ sở tri thức tìm kiếm
- [x] Multi-language support
- [x] Chat history

### 👨‍⚕️ Expert Consultation
- [x] Danh sách chuyên gia
- [x] Chat trực tiếp với chuyên gia
- [x] Gửi câu hỏi và hình ảnh
- [x] Rating và feedback
- [x] Lịch sử tư vấn
- [x] Push notifications

### 📊 Reports & Analytics
- [x] Dashboard thống kê
- [x] Báo cáo sức khỏe
- [x] Thống kê chi phí
- [x] Biểu đồ tăng trưởng
- [x] Offline reports

### 🌤️ Weather Integration
- [x] Weather widget
- [x] Location-based weather
- [x] Weather alerts
- [x] Care recommendations
- [x] Historical weather data

### 📱 Mobile Features
- [x] Offline mode
- [x] Accessibility support
- [x] Background sync

---

## 🛠️ Tech Stack

### Core Technologies
- **Language**: Kotlin 100%
- **UI Framework**: Jetpack Compose
- **Architecture**: MVVM + Repository Pattern
- **DI**: Hilt (Dagger)
- **Async**: Kotlin Coroutines + Flow
- **Database**: Room (SQLite)
- **Network**: Retrofit2 + OkHttp3
- **Image Loading**: Coil
- **JSON**: Gson/Moshi

### UI/UX Libraries
- **Material Design 3**: Material You
- **Navigation**: Navigation Compose
- **Charts**: MPAndroidChart
- **Camera**: CameraX
- **QR Code**: ZXing
- **Biometric**: BiometricPrompt
- **Permissions**: Accompanist Permissions

### Networking & Data
- **API Client**: Retrofit2
- **HTTP Logging**: OkHttp Logging Interceptor
- **Caching**: OkHttp Cache
- **Serialization**: Gson
- **Image Upload**: Multipart requests

### Development Tools
- **Build System**: Gradle Kotlin DSL
- **Code Quality**: Detekt + Ktlint
- **Testing**: JUnit5 + MockK + Compose Testing
- **CI/CD**: GitHub Actions
- **Crash Reporting**: Firebase Crashlytics
- **Analytics**: Firebase Analytics

---

## 📦 Cài đặt và chạy dự án

### Yêu cầu hệ thống
- **Android Studio**: Arctic Fox (2020.3.1) hoặc mới hơn
- **JDK**: 11 hoặc 17
- **Android SDK**: API 24+ (Android 7.0)
- **Target SDK**: API 34 (Android 14)
- **Min SDK**: API 24 (Android 7.0)
- **Kotlin**: 1.9.0+

### 1. Clone repository
```bash
git clone https://github.com/manhkaka/antrai-android.git
cd antrai-android
```

### 2. Mở project trong Android Studio
```bash
# Mở Android Studio và chọn "Open an existing project"
# Chọn thư mục antrai-android
```

### 3. Cấu hình Backend API
Tạo file `local.properties` trong thư mục root:
```properties
# Backend API Configuration
API_BASE_URL=http://10.0.2.2:3000/api
# Hoặc URL production: https://your-api-domain.com/api

# Development settings
DEBUG_MODE=true
LOG_LEVEL=DEBUG
```

### 4. Cấu hình Firebase (Optional)
```bash
# Tải file google-services.json từ Firebase Console
# Đặt vào app/google-services.json
```

### 5. Build và chạy
```bash
# Debug build
./gradlew assembleDebug

# Release build
./gradlew assembleRelease

# Chạy tests
./gradlew test

# Lint check
./gradlew lint
```

### 6. Cài đặt APK
```bash
# Cài đặt debug APK
adb install app/build/outputs/apk/debug/app-debug.apk

# Hoặc chạy trực tiếp từ Android Studio
# Click "Run" button hoặc Shift + F10
```

---

## 📱 Screenshots & UI Preview

### Main Screens
- **Login/Register**: Material Design 3 với biometric support
- **Dashboard**: Cards layout với health overview
- **Poultry List**: RecyclerView với search & filter
- **Poultry Detail**: Tabbed layout với images
- **AI Chat**: Chat interface với voice input
- **Expert Chat**: Real-time messaging
- **Reports**: Charts và statistics
- **Settings**: Theme, language, notifications

### Design System
- **Colors**: Material You dynamic colors
- **Typography**: Roboto font family
- **Icons**: Material Design Icons
- **Components**: Custom Compose components
- **Animations**: Smooth transitions và micro-interactions

---

## 🔧 Development Setup

### Project Structure
```
antrai-android/
├── app/                           # Main app module
├── core/                          # Core utilities
├── data/                          # Data layer module
├── domain/                        # Domain layer module
├── ui/                           # UI components module
├── buildSrc/                      # Build configuration
├── gradle/                        # Gradle wrapper
├── .github/                       # GitHub Actions
├── .idea/                         # Android Studio settings
├── docs/                          # Documentation
└── README_2.md                    # This file
```

### Build Variants
```kotlin
buildTypes {
    debug {
        isDebuggable = true
        applicationIdSuffix = ".debug"
        versionNameSuffix = "-debug"
    }
    
    release {
        isMinifyEnabled = true
        proguardFiles(getDefaultProguardFile("proguard-android-optimize.txt"), "proguard-rules.pro")
    }
}
```

### Code Quality
```bash
# Format code
./gradlew ktlintFormat

# Check code style
./gradlew ktlintCheck

# Run detekt
./gradlew detekt

# Run all checks
./gradlew check
```

---

## 🧪 Testing

### Test Structure
```
app/src/test/                      # Unit tests
app/src/androidTest/               # Instrumented tests
├── java/com/antrai/
│   ├── data/                      # Data layer tests
│   ├── domain/                    # Domain layer tests
│   ├── ui/                        # UI tests
│   └── utils/                     # Utility tests
```

### Running Tests
```bash
# Unit tests
./gradlew test

# Instrumented tests
./gradlew connectedAndroidTest

# All tests
./gradlew check

# Test coverage
./gradlew jacocoTestReport
```

### Test Coverage
- **Unit Tests**: > 80% coverage
- **Integration Tests**: Critical user flows
- **UI Tests**: Main screens và navigation
- **Performance Tests**: Memory và CPU usage

---

## 📈 Performance & Optimization

### Performance Metrics
- **App Launch Time**: < 2 seconds
- **Screen Transition**: < 300ms
- **API Response**: < 2 seconds
- **Memory Usage**: < 150MB
- **Battery Usage**: Optimized for all-day use

### Optimization Techniques
- **Image Optimization**: WebP format, lazy loading
- **Database**: Room with proper indexing
- **Network**: Request caching, compression
- **UI**: Compose recomposition optimization
- **Memory**: Proper lifecycle management
- **Battery**: Background task optimization

---

## 🔒 Security

### Data Protection
- **API Security**: JWT token management
- **Local Storage**: Encrypted SharedPreferences
- **Biometric**: Secure authentication
- **Network**: Certificate pinning
- **Code Obfuscation**: ProGuard/R8

### Privacy
- **Permissions**: Minimal required permissions
- **Data Collection**: Transparent privacy policy
- **User Consent**: Clear opt-in/opt-out
- **Data Retention**: Automatic cleanup

---

## 🚀 Deployment

### Build Configuration
```kotlin
android {
    compileSdk = 34
    
    defaultConfig {
        applicationId = "com.antrai.poultry"
        minSdk = 24
        targetSdk = 34
        versionCode = 1
        versionName = "1.0.0"
    }
    
    signingConfigs {
        create("release") {
            // Release signing configuration
        }
    }
}
```

### Release Process
1. **Version Bump**: Update version code/name
2. **Build**: Generate signed APK/AAB
3. **Testing**: Internal testing
4. **Upload**: Google Play Console
5. **Release**: Staged rollout

### Distribution
- **Google Play Store**: Primary distribution
- **APK Download**: Direct download option
- **Beta Testing**: Internal/Closed testing
- **Staged Rollout**: Gradual release

---

## 🤝 Contributing

### Development Workflow
1. Fork repository
2. Create feature branch: `git checkout -b feature/amazing-feature`
3. Make changes và commit: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Create Pull Request

### Code Standards
- **Kotlin**: Official style guide
- **Compose**: Material Design guidelines
- **Architecture**: Clean Architecture principles
- **Testing**: TDD approach
- **Documentation**: KDoc comments

---

## 📄 License

Dự án này được phát hành dưới [MIT License](LICENSE).

---

## 👥 Team

- **Android Developer**: [ManhKa]
- **UI/UX Designer**: [ManhKa]
- **Backend Integration**: AnTrai Backend Team
- **QA Tester**: [Tester Name]

---

## 📞 Support & Contact

- **Email**: android-support@antrai.com
- **Documentation**: [Android Docs](docs/)
- **Issues**: [GitHub Issues](https://github.com/manhkaka/antrai-android/issues)
- **Discussions**: [GitHub Discussions](https://github.com/manhkaka/antrai-android/discussions)

---

## 🎯 Roadmap

### Phase 1 (Current)
- [x] Core app structure
- [x] Authentication flow
- [x] Basic poultry management
- [x] AI chat integration

### Phase 2 (Next)
- [ ] Advanced AI features
- [ ] Real-time notifications
- [ ] Offline sync improvements
- [ ] Tablet optimization

### Phase 3 (Future)
- [ ] Wear OS companion app
- [ ] AR features for health diagnosis
- [ ] IoT device integration
- [ ] Multi-tenant support

---

## 📚 Additional Resources

### Documentation
- [Android Developer Guide](https://developer.android.com/)
- [Jetpack Compose](https://developer.android.com/jetpack/compose)
- [Material Design 3](https://m3.material.io/)
- [Kotlin Documentation](https://kotlinlang.org/docs/)

### Backend API
- [API Documentation](http://localhost:3000/api-docs)
- [Postman Collection](docs/postman/)
- [API Testing Guide](docs/api-testing.md)

---

<div align="center">

**🐔 AnTrai Android App - Smart Poultry Management**

*Empowering farmers with intelligent mobile poultry management*

[![Made with ❤️](https://img.shields.io/badge/Made%20with-❤️-red?style=flat)](https://github.com/manhkaka/antrai-android)
[![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=flat&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=flat&logo=android&logoColor=white)](https://developer.android.com/)

</div>
