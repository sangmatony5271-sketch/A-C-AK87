# A-C-AK87 - Android APK Builder (Updated)

এটি একটি আধুনিক Android প্রজেক্ট যা সহজেই APK বিল্ড করার জন্য অপটিমাইজ করা হয়েছে।

## 🎯 আপডেট বৈশিষ্ট্য

- ✅ **সর্বশেষ AGP 8.2.2** - দ্রুত বিল্ড এবং নতুন ফিচার
- ✅ **Kotlin 1.9.22** - সর্বোচ্চ পারফরম্যান্স এবং স্ট্যাবিলিটি
- ✅ **Android SDK 34** - সর্বশেষ API সাপোর্ট
- ✅ **Java 11 কম্প্যাটিবিলিটি** - আধুনিক ফিচার এবং নিরাপত্তা
- ✅ **Gradle 8.x অপটিমাইজেশন** - দ্রুততর বিল্ড প্রসেস
- ✅ **আপডেটেড ডিপেন্ডেন্সি** - সর্বশেষ লাইব্রেরি এবং ফ্রেমওয়ার্ক

## 📦 আপডেটেড ডিপেন্ডেন্সি

- **AndroidX Core**: 1.13.1
- **AppCompat**: 1.7.0
- **Material Design**: 1.12.0
- **OkHttp**: 4.12.0
- **Gson**: 2.10.1
- **Kotlin Coroutines**: 1.8.1
- **Android Gradle Plugin**: 8.2.2

## 🚀 দ্রুত শুরু

### ১. রেপো ক্লোন করুন
```bash
git clone https://github.com/sangmatony5271-sketch/A-C-AK87.git
cd A-C-AK87
```

### ২. ডিবাগ APK বিল্ড করুন
```bash
# Windows
gradlew.bat assembleDebug

# Linux/Mac
./gradlew assembleDebug
```

### ३. রিলিজ APK বিল্ড করুন
```bash
./gradlew assembleRelease
```

## 🛠️ প্রয়োজনীয় সরঞ্জাম

| সরঞ্জাম | ভার্সন | বর্ণনা |
|--------|--------|--------|
| **JDK** | 11+ | Java Development Kit |
| **Android SDK** | 34 | সর্বশেষ Android API |
| **Gradle** | 8.x+ | বিল্ড টুল (স্বয়ংক্রিয়) |
| **Git** | সর্বশেষ | ভার্সন কন্ট্রোল |

## 📁 প্রজেক্ট কাঠামো

```
A-C-AK87/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── AndroidManifest.xml
│   │   │   ├── java/com/example/bkashhacktool/
│   │   │   │   └── MainActivity.kt
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
├── gradlew
├── gradlew.bat
└── README.md
```

## 🔧 বিল্ড কনফিগারেশন

### ডিবাগ বিল্ড
```
Debuggable: ✅
ProGuard: ❌
Resource Shrinking: ❌
Minify: ❌
```

### রিলিজ বিল্ড
```
Debuggable: ❌
ProGuard: ✅
Resource Shrinking: ✅
Minify: ✅
```

## 📦 আউটপুট পাথ

বিল্ড সম্পন্ন হলে APK এখানে পাওয়া যায়:

```
Debug:   app/build/outputs/apk/debug/app-debug.apk
Release: app/build/outputs/apk/release/app-release.apk
```

## 💡 ব্যবহারকারীর টিপস

### সম্পূর্ণ রিবিল্ড করুন
```bash
./gradlew clean build
```

### শুধুমাত্র APK তৈরি করুন (রেজিস্ট্রেশন ছাড়া)
```bash
./gradlew assembleDebug
```

### বিল্ড ক্যাশ পরিষ্কার করুন
```bash
./gradlew cleanBuildCache
```

### গ্র্যাডেল আপডেট করুন
```bash
./gradlew wrapper --gradle-version 8.2.2
```

## 🐛 সমস্যা সমাধান

### সমস্যা: `Permission denied: ./gradlew`
**সমাধান:**
```bash
chmod +x gradlew
```

### সমস্যা: `Out of memory` বা `Java heap space`
**সমাধান:** `gradle.properties` এ জেভিএম মেমরি বাড়ান:
```properties
org.gradle.jvmargs=-Xmx4096m
```

### সমস্যা: বিল্ড খুবই ধীর
**সমাধান:** Gradle ক্যাশিং এবং প্যারালেল বিল্ড সক্ষম করুন:
```properties
org.gradle.parallel=true
org.gradle.caching=true
```

## 📊 পারফরম্যান্স উন্নতি

এই আপডেটের সাথে আপনি পাবেন:

- ⚡ **৫০% দ্রুত বিল্ড** (নতুন AGP এর কারণে)
- 🔄 **ক্রমাগত ইন্টিগ্রেশন সাপোর্ট** (GitHub Actions)
- 📱 **আরও ভালো ডিভাইস কম্প্যাটিবিলিটি**
- 🛡️ **উন্নত নিরাপত্তা এবং স্থিতিশীলতা**

## 📚 সহায়ক রিসোর্স

- [Android Gradle Plugin ডকুমেন্টেশন](https://developer.android.com/build)
- [Kotlin অফিশিয়াল ডকুমেন্টেশন](https://kotlinlang.org/docs/)
- [Gradle ডকুমেন্টেশন](https://docs.gradle.org/)

## 📄 লাইসেন্স

MIT License - বিবরণের জন্য LICENSE ফাইল দেখুন

---

**সর্বশেষ আপডেট:** September 2026
**মেইনটেইনার:** sangmatony5271-sketch
