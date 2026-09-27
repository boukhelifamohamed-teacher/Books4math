# كتب الرياضيات - المتوسط | VoltBuilder

هذه النسخة مخصصة للرفع إلى VoltBuilder بصيغة Apache Cordova، وليست نسخة Capacitor.

## بنية المشروع
- config.xml
- voltbuilder.json
- www/index.html
- resources/iconTemplate.png
- resources/splashTemplate.png
- resources/resources.json

VoltBuilder يعتمد ملف ZIP واحدًا بهذه البنية، ويمكنه توليد مقاسات أيقونة وشاشة البداية تلقائيًا من ملفات القوالب.

## من الهاتف
1. فك الضغط فقط إذا أردت فحص الملفات؛ لا تغيّر بنية المجلد.
2. ارفع ملف ZIP إلى صفحة Upload في VoltBuilder.
3. اختر iOS.
4. لإخراج IPA قابل للتثبيت، يجب أن يكون لديك حساب Apple Developer وشهادات iOS المناسبة.
5. ضع ملفات الشهادة داخل مجلد `certificates` وأسماءها في `voltbuilder.json` حسب تعليمات VoltBuilder.

## ملاحظة
هذه النسخة لا تحتوي على شهادات Apple أو كلمات مرورها لأسباب أمنية.
