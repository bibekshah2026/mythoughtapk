# My Thoughts — Android App
**Blog:** https://blog.ervivekshah.com.np  
**Package:** com.vivekshah.mythoughts  
**Version:** 1.0

---

## ✨ App Features
- 🌐 Full WebView of your blog
- 🔄 Pull-to-refresh
- 📶 Offline detection with Retry button
- ↩️ Back navigation within the blog
- 🔗 External links open in browser
- 📤 Share current post
- 🌙 Splash screen with animation (matches your blog's dark purple #0a0323 theme)
- 🏠 Home / Share / Open in Browser / About menu

---

## 🛠️ How to Build the APK

### Step 1 — Install Prerequisites
1. Download **Android Studio**: https://developer.android.com/studio
2. Install it (includes Java JDK automatically)
3. Open Android Studio → wait for Gradle to finish downloading

### Step 2 — Open the Project
1. Open Android Studio
2. Click **"Open"** (not "New Project")
3. Navigate to and select the `MyThoughtsApp` folder
4. Click **OK**
5. Wait for Gradle sync to complete (may take 2–5 minutes first time)

### Step 3 — Build Debug APK (for testing)
- In Android Studio menu: **Build → Build Bundle(s) / APK(s) → Build APK(s)**
- OR press `Ctrl+F9` (Windows/Linux) / `Cmd+F9` (Mac)
- Output location: `app/build/outputs/apk/debug/app-debug.apk`

### Step 4 — Build Release APK (for distribution)
1. **Build → Generate Signed Bundle / APK**
2. Choose **APK**
3. Click **"Create new..."** to make a keystore (save this file safely!)
4. Fill in keystore details, click Next
5. Choose **release**, check both V1 and V2 signature
6. Click **Finish**
7. Output: `app/build/outputs/apk/release/app-release.apk`

---

## 📱 Install on Your Phone
- Enable **Developer Options** on your Android phone
- Turn on **USB Debugging**
- Connect phone via USB → Android Studio will detect it
- Click the ▶️ **Run** button to install directly

OR transfer the APK file to your phone and open it to install
(Settings → Allow installation from unknown sources)

---

## 🎨 Customization
| File | What to change |
|------|----------------|
| `values/colors.xml` | App colors (`splash_bg` = #0a0323 matches your blog) |
| `drawable/ic_logo.xml` | App icon (vector graphic) |
| `MainActivity.kt` line ~19 | `BLOG_URL` — change the blog URL |
| `values/strings.xml` | App name |

---

## 📦 Requirements
- Android Studio Hedgehog (2023.1) or newer
- JDK 17+ (bundled with Android Studio)
- Android SDK 34
- Min Android version supported: Android 5.0 (API 21) — covers 99%+ of devices
