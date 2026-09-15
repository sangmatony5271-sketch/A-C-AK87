# A-C-AK87 - Android APK Builder

এটি একটি Android প্রজেক্ট যা অটো এবং ম্যানুয়াল উভয় পদ্ধতিতে APK বিল্ড করার সুবিধা প্রদান করে।

## 🎯 বৈশিষ্ট্য

- ✅ **অটো বিল্ড অপশন** (GitHub Actions সহ)
- ✅ **ম্যানুয়াল বিল্ড অপশন** (স্থানীয় বা ওয়ার্কফ্লো ডিসপ্যাচ)
- ✅ **ডিবাগ এবং রিলিজ বিল্ড** সাপোর্ট
- ✅ **এপিকে স্বয়ংক্রিয় আপলোড**
- ✅ **একাধিক বিল্ড ভেরিয়েন্ট** (Standard, Beta)

## 📱 বিল্ড করার উপায়

### 1️⃣ GitHub Actions এ অটো বিল্ড
প্রতিটি পুশের সাথে স্বয়ংক্রিয়ভাবে APK তৈরি হয়।

### 2️⃣ ���্যানুয়াল বিল্ড (ওয়ার্কফ্লো ডিসপ্যাচ)
`GitHub Actions > Android Build > "Run workflow"` ক্লিক করুন।

### 3️⃣ স্থানীয় বিল্ড
```bash
# ডিবাগ APK তৈরি করুন
./gradlew assembleDebug

# রিলিজ APK তৈরি করুন
./gradlew assembleRelease

# Standard ফ্লেভারে বিল্ড করুন
./gradlew assembleStandardDebug
./gradlew assembleStandardRelease

# Beta ফ্লেভারে বিল্ড করুন
./gradlew assembleBetaDebug
./gradlew assembleBetaRelease
```

## 🛠️ প্রয়োজনীয় সরঞ্জাম

- **JDK 11** বা তার উপরে
- **Android SDK** (API 33+)
- **Gradle** (স্বয়ংক্রিয়ভাবে ডাউনলোড হয়)
- **Git**

## 📝 প্রজেক্ট কাঠামো

```
A-C-AK87/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── AndroidManifest.xml
│   │   │   ├── java/com/example/akapp/
│   │   │   │   └── MainActivity.java
│   │   │   └── res/
│   │   │       ├── layout/
│   │   │       ├── values/
│   │   │       └── mipmap/
│   │   ├── debug/
│   │   └── release/
│   └── build.gradle
├── build.gradle
├── settings.gradle
├── gradle.properties
└── README.md
```

## 🔧 বিল্ড কনফিগারেশন

### Debug বিল্ড
- Debuggable: ✅
- ProGuard: ❌
- Minify: ❌

### Release বিল্ড
- Debuggable: ❌
- ProGuard: ✅
- Minify: ✅

## 📦 আউটপুট

বিল্ড সম্পন্ন হলে APK ফাইল এখানে পাওয়া যায়:
```
app/build/outputs/apk/{variant}/{buildType}/app-{variant}-{buildType}.apk
```

উদাহরণ:
- `app/build/outputs/apk/standard/debug/app-standard-debug.apk`
- `app/build/outputs/apk/standard/release/app-standard-release.apk`
- `app/build/outputs/apk/beta/debug/app-beta-debug.apk`
- `app/build/outputs/apk/beta/release/app-beta-release.apk`

## 🚀 দ্রুত শুরু

1. **রেপো ক্লোন করুন:**
   ```bash
   git clone https://github.com/sangmatony5271-sketch/A-C-AK87.git
   cd A-C-AK87
   ```

2. **ডিবাগ APK তৈরি করুন:**
   ```bash
   ./gradlew assembleDebug
   ```

3. **APK স্থাপন করুন (অ্যান্ড্রয়েড ডিভাইসে):**
   ```bash
   adb install app/build/outputs/apk/standard/debug/app-standard-debug.apk
   ```

## 📄 লাইসেন্স

MIT License - বিবরণের জন্য LICENSE ফাইল দেখুন
