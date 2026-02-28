
buildscript {
    repositories { google(); mavenCentral() }
    dependencies {
        classpath 'com.android.tools.build:gradle:8.2.0'
        classpath 'org.jetbrains.kotlin:kotlin-gradle-plugin:1.9.22'
    }
}
allprojects { repositories { google(); mavenCentral() } }

#!/bin/bash
# Togaff VPN APK Build Script
# Requirements: Android Studio with Android SDK installed

echo "=== Togaff VPN APK Builder ==="
echo ""
echo "Option 1: Android Studio (recommended)"
echo "  1. Open Android Studio"
echo "  2. File -> Open -> select this folder"
echo "  3. Build -> Build Bundle(s)/APK(s) -> Build APK(s)"
echo "  4. APK will be in app/build/outputs/apk/debug/"
echo ""
echo "Option 2: Command line (needs Android SDK)"
echo "  export ANDROID_HOME=~/Android/Sdk"
echo "  ./gradlew assembleDebug"
echo "  # APK: app/build/outputs/apk/debug/app-debug.apk"
echo ""
echo "Option 3: Online builder"
echo "  1. Zip this entire folder"
echo "  2. Upload to https://appetize.io or use GitHub Actions"

## This file must *NOT* be checked into Version Control Systems,
# as it contains information specific to your local configuration.
#
# Location of the SDK. This is only used by Gradle.
# For customization when using a Version Control System, please read the
# header note.
#Sat Feb 28 17:06:51 YEKT 2026
sdk.dir=C\:\\Users\\\u041A\u0430\u0440\u043E\u043B\u0438\u043D\u0430\\AppData\\Local\\Android\\Sdk

rootProject.name = "TogaffVPN"
include ':app'
