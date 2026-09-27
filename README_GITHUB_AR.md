# 📱 كتب الرياضيات – مشروع GitHub Actions

هذه النسخة مجهزة لتعمل من الهاتف عبر GitHub Actions.

## الاستخدام من الهاتف

1. أنشئ Repository جديدًا في GitHub.
2. ارفع **محتويات هذا ZIP** إلى المستودع، وليس ملف ZIP نفسه داخل المستودع.
3. اجعل المستودع Public إذا كنت تريد الاستفادة من GitHub-hosted standard runners المجانية للمستودعات العامة.
4. افتح تبويب **Actions**.
5. اختر **Build iOS App**.
6. اضغط **Run workflow**.
7. بعد انتهاء البناء افتح نتيجة التشغيل ثم **Artifacts**.
8. ستجد:
   - `MathMiddle-unsigned.ipa`
   - `MathMiddle.app`

## مهم جدًا

ملف `MathMiddle-unsigned.ipa` الناتج من هذا المسار هو **غير موقّع**. وجود IPA لا يعني أنه يمكن تثبيته مباشرة على iPhone.

للتثبيت على iPhone أو التوزيع، يلزم توقيع Apple مناسب. GitHub توثق أن توقيع تطبيقات iOS على macOS runners يحتاج شهادة Apple وProvisioning Profile محفوظين كـ GitHub Secrets.

لا تضع شهادات Apple أو كلمات المرور داخل ملفات المشروع.

## لماذا هذه النسخة مجانية؟

الـ workflow يستخدم `macos-latest` في GitHub Actions. GitHub توضح أن standard GitHub-hosted runners للمستودعات العامة مجانية وغير محدودة وفق شروطها الحالية.

لكن هذا لا يجعل حساب Apple Developer أو شهادات التوقيع مجانية.

## بيانات التطبيق

الاسم: كتب الرياضيات - المتوسط
Bundle ID: dz.boukhlifa.mathmiddle
المصمم: الأستاذ بوخليفة محمد

## الملفات المهمة

`.github/workflows/build-ios.yml`
Workflow البناء التلقائي.

`www/index.html`
واجهة التطبيق.

`config.xml`
إعدادات Cordova.

`resources/`
الشعار وشاشة البداية.

