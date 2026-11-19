# JP Chat — Android Demo Project

এটি JP Chat অ্যাপের **শুরুর ডেমো সোর্স কোড**। এখন এতে ডার্ক UI, চ্যাট তালিকা, ডেমো কথোপকথন এবং লোকালি মেসেজ দেখানোর নমুনা আছে।

## গুরুত্বপূর্ণ
- এটি APK নয়; Android Studio/Gradle দিয়ে build করতে হবে।
- এই ডেমোতে অনলাইনে মেসেজ পাঠানো হয় না।
- Login/OTP, Firebase, ব্যক্তিগত chat database, notification, media sharing এবং audio/video call এখনো যুক্ত হয়নি।
- কোনো বাস্তব ফোন নম্বর বা পাসওয়ার্ড কোডে লিখবে না।

## Build করার জন্য
Android Studio-তে এই ফোল্ডারটি Open করে Gradle Sync করো, তারপর Build > Build APK(s) নির্বাচন করো।
Android Studio-র উপযুক্ত JDK/SDK লাগবে। 2GB RAM ফোনে Android Studio চালানো কঠিন হতে পারে; কম্পিউটার বা ক্লাউড বিল্ড পরিবেশ সুবিধাজনক।

## Package
`com.jpchat.app`
## ফোন থেকে GitHub দিয়ে APK Build
1. GitHub-এ নতুন repository তৈরি করো; নাম দাও `JP-Chat` এবং Public বা Private যেকোনোটি রাখতে পারো।
2. এই ZIP extract করে সব ফাইল repository-তে upload করো। `.github/workflows/build.yml` ফাইলটিও অবশ্যই upload হবে।
3. `main` branch-এ ফাইলগুলো commit করো।
4. repository-র Actions tab খুলে `Build JP Chat APK` workflow নির্বাচন করো।
5. `Run workflow` চাপো; build শেষ হলে সফল run খুলে Artifacts থেকে `JP-Chat-debug-APK` ডাউনলোড করো।
6. ZIP artifact extract করে `app-debug.apk` ফাইলটি Android-এ ইনস্টল করো।

GitHub Actions-এ build করতে internet connection লাগবে. Debug APK test build; Play Store release-এর signed APK নয়.
