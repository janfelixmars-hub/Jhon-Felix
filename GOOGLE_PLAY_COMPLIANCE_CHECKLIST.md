# Google Play Store Compliance Checklist

This document outlines the compliance status of the Mood Wellness and Recipe app for Google Play Store submission.

## ✅ Completed Requirements

### 1. Package Name
- **Status**: ✅ Fixed
- **Previous**: `com.example.flutter_application_1` (violates Google Play policy)
- **Current**: `com.moodwellness.recipe` (compliant)
- **Files Updated**:
  - `android/app/build.gradle.kts`
  - `android/app/src/main/AndroidManifest.xml`
  - `android/app/src/main/kotlin/com/moodwellness/recipe/MainActivity.kt`
  - `android/app/google-services.json`

### 2. App Information
- **App Name**: "Mood Wellness and Recipe" ✅
- **Description**: Updated in `pubspec.yaml` ✅
- **App Icon**: Configured ✅

### 3. Permissions
- **Notification Permissions**: Properly declared and used ✅
- **Image Picker**: Properly declared and used ✅
- **Internet Permission**: Only in debug/profile builds (acceptable) ✅

### 4. Privacy Policy
- **Status**: ✅ Created
- **Location**: `PRIVACY_POLICY.md`
- **Note**: You must host this online and provide the URL in Google Play Console

### 5. Data Handling
- **Local Storage Only**: All data stored locally ✅
- **No Data Transmission**: App works offline ✅
- **No Third-Party Analytics**: No tracking implemented ✅

## ⚠️ Action Items Required Before Submission

### 1. Firebase Configuration
- **Status**: ⚠️ Requires Manual Update
- **Action Required**: 
  1. Go to [Firebase Console](https://console.firebase.google.com/)
  2. Select your project: `mood-wellness-app-21463`
  3. Go to Project Settings > Your Apps
  4. Update the Android app package name from `com.example.flutter_application_1` to `com.moodwellness.recipe`
  5. Download the new `google-services.json` file
  6. Replace the existing file in `android/app/google-services.json`

### 2. Privacy Policy URL
- **Status**: ⚠️ Requires Hosting
- **Action Required**:
  1. Host the `PRIVACY_POLICY.md` file on a website (GitHub Pages, your website, etc.)
  2. Update the email and website placeholders in the privacy policy
  3. Provide the URL in Google Play Console under "Store listing" > "Privacy Policy"

### 3. App Signing
- **Status**: ⚠️ Requires Setup
- **Action Required**:
  1. Generate a release keystore (if not already done)
  2. Configure signing in `android/app/build.gradle.kts`
  3. Remove debug signing config from release builds

### 4. Content Rating
- **Status**: ⚠️ Requires Submission
- **Action Required**: Complete the content rating questionnaire in Google Play Console

### 5. Store Listing
- **Status**: ⚠️ Requires Completion
- **Action Required**:
  - App description (short and full)
  - Screenshots (phone and tablet)
  - Feature graphic
  - Promotional text
  - Category selection

### 6. Target Audience
- **Status**: ⚠️ Requires Declaration
- **Action Required**: Declare target audience and content appropriateness in Google Play Console

## 📋 Google Play Policy Compliance

### ✅ User Data Privacy
- **Local Storage Only**: All data stored on device ✅
- **No Data Collection**: No personal data transmitted ✅
- **Privacy Policy**: Created and ready for hosting ✅

### ✅ Permissions
- **Justified Permissions**: All permissions are necessary and properly declared ✅
- **Runtime Permissions**: Notification permissions requested at runtime ✅

### ✅ Content Policies
- **No Prohibited Content**: App contains no prohibited content ✅
- **Appropriate Content**: Wellness and recipe management app ✅

### ✅ Technical Requirements
- **Target SDK**: Configured ✅
- **Min SDK**: Configured ✅
- **64-bit Support**: Flutter apps support 64-bit by default ✅

### ✅ Monetization
- **No Ads**: App does not contain advertisements ✅
- **No In-App Purchases**: Currently no IAP implemented ✅

## 🔍 Additional Recommendations

### 1. App Store Optimization (ASO)
- Create compelling app description
- Use relevant keywords
- Add high-quality screenshots
- Create promotional video (optional)

### 2. Testing
- Test on multiple Android devices
- Test on different Android versions
- Verify all features work correctly
- Test notification functionality

### 3. Legal
- Review privacy policy with legal counsel (if applicable)
- Ensure compliance with local data protection laws
- Add contact information for user support

### 4. Support
- Set up support email
- Create FAQ document
- Prepare for user feedback

## 📝 Pre-Submission Checklist

Before submitting to Google Play Store, ensure:

- [ ] Package name updated to `com.moodwellness.recipe`
- [ ] Firebase project updated with new package name
- [ ] New `google-services.json` downloaded and placed in `android/app/`
- [ ] Privacy policy hosted online and URL available
- [ ] App signing configured for release builds
- [ ] App tested on multiple devices
- [ ] All features working correctly
- [ ] Store listing information prepared
- [ ] Screenshots and graphics ready
- [ ] Content rating questionnaire completed
- [ ] Support email configured

## 🚨 Important Notes

1. **Package Name Change**: Once you publish an app with a package name, you cannot change it. The package name `com.moodwellness.recipe` is now set and should be used for all future updates.

2. **Firebase**: You must update the Firebase project settings to match the new package name. The app will not work with Firebase until this is done.

3. **Privacy Policy**: Google Play requires a publicly accessible privacy policy URL. You cannot submit without it.

4. **App Signing**: For production releases, you must use a release keystore, not the debug keystore.

## 📞 Support

If you encounter any issues during the submission process, refer to:
- [Google Play Console Help](https://support.google.com/googleplay/android-developer)
- [Google Play Policy Center](https://play.google.com/about/developer-content-policy/)

---

**Last Updated**: [Current Date]
**App Version**: 1.0.0+1
**Package Name**: com.moodwellness.recipe

