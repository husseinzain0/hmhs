# HMH System — تطبيق مستقل

## أندرويد (APK) — الشريحة 1/2/3/4 تعمل فعلياً
المتطلبات: Node.js 18+ ، JDK 17 ، Android Studio (أو Android SDK).

    npm run setup     # تثبيت + إنشاء مشروع أندرويد + إضافة الاتصال بالشريحة
    npm run apk       # بناء APK  →  android/app/build/outputs/apk/debug/app-debug.apk
    # أو: npm run open  ثم Build > Build APK(s) من Android Studio

بعد تعديل www/index.html شغّل: npm run sync

ملاحظات:
- عند أول اتصال سيطلب التطبيق إذن الهاتف، وافق عليه.
- SIM 3 و SIM 4 تعملان فقط إن كان هاتفك يدعم أكثر من شريحتين؛ وإلا تظهر رسالة «غير متاحة» ويفتح الاتصال العادي.
- الـ APK هنا debug (للتثبيت المباشر). للنشر في المتجر وقّعه من Android Studio.

## ويندوز / ماك (Electron)
    cd desktop
    npm install
    npm start             # تجربة
    npm run build:win     # على ويندوز  → dist/
    npm run build:mac     # على ماك     → dist/ (.dmg)
(بناء ماك يتطلب جهاز ماك.) تنبيه: أجهزة الحاسوب بلا شرائح اتصال، فأزرار الاتصال هناك تفتح tel: فقط.
