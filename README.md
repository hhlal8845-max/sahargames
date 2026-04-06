# 🎮 sahar-games — تحويل لتطبيق Android/iOS

## المتطلبات
- [Node.js](https://nodejs.org) (v18+)
- Android Studio (للأندرويد)
- Xcode على Mac (للـ iOS)

---

## خطوات التثبيت

### 1️⃣ فتح المجلد وتثبيت الحزم
```bash
cd sahar-games
npm install
```

### 2️⃣ إضافة المنصات
```bash
# أندرويد
npx cap add android

# iOS (على Mac فقط)
npx cap add ios
```

### 3️⃣ مزامنة الملفات
```bash
npx cap sync
```

### 4️⃣ فتح المشروع
```bash
# أندرويد - يفتح Android Studio
npx cap open android

# iOS - يفتح Xcode
npx cap open ios
```

---

## بناء APK (أندرويد)
1. افتح Android Studio
2. `Build` → `Generate Signed Bundle / APK`
3. اختر APK وأكمل الخطوات

## نشر على Google Play
1. `Build` → `Generate Signed Bundle / APK` → اختر **Android App Bundle (.aab)**
2. ارفع الـ `.aab` على Google Play Console

---

## ملاحظات مهمة
- فيسبوك Login يشتغل بس لو ضفت `SHA-1` fingerprint في إعدادات Facebook App
- تأكد تضيف `com.sahargames.app` كـ Package Name في Facebook Developer Console
- إذا بدك تغير الـ App ID، عدّله في `capacitor.config.json` → `appId`
