# DOUKAN AL HAY OFFLINE v2

برنامج مستقل لمحل مواد غذائية، يعمل محلياً بدون إنترنت بعد التثبيت.

## يحتوي على
- Caisse / البيع وإنقاص المخزون تلقائياً
- المنتجات والمخزون والبحث والكودبار
- قارئ كودبار مستقل عن Caisse (USB/Bluetooth أو تصوير عند دعم الجهاز)
- 200 منتج جاهز للتحميل
- المشتريات وإدخال السلع
- الموردون
- المصاريف
- تقارير اليوم والشهر وكل المبيعات والربح التقريبي
- نسخة احتياطية واسترجاع JSON
- تصدير CSV
- PC عبر Electron
- Android عبر Capacitor

## مهم
المشروع نفسه Offline عند التشغيل ولا يعتمد على GitHub أو موقع ويب. الإنترنت مطلوب فقط أثناء **مرحلة بناء وتثبيت** الحزم (npm/Gradle) على جهاز التطوير. بعد إنشاء البرنامج APK أو نسخة PC، يمكن تشغيله في المحل بدون إنترنت.

## PC
1. ثبّت Node.js LTS على Windows.
2. افتح CMD داخل مجلد المشروع.
3. نفّذ: `npm install`
4. للتجربة: `npm run desktop`
5. لإنشاء مثبت Windows: `npm run desktop:build`

## Android
1. نفّذ `npm install` ثم `npm run android:add` مرة واحدة.
2. نفّذ `npm run android:sync`.
3. افتح Android Studio بواسطة `npm run android:open`.
4. ابنِ APK Debug أو Release من Android Studio.

لا ترفع مجلد `android` الناتج إلى GitHub إذا كان الهدف فقط حفظ المصدر؛ يمكن توليده بواسطة Capacitor.
