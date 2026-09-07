# بناء APK لتطبيق ذِكر

## Codemagic
هذا المشروع مجهز بملف `codemagic.yaml`.

1. ارفع محتويات المشروع إلى GitHub (وليس ملف ZIP داخل المستودع).
2. اربط المستودع مع Codemagic.
3. اختر Workflow: `dhikr-android`.
4. اضغط Start new build.
5. بعد انتهاء البناء ستجد APK ضمن Artifacts.

سيتم بناء:
- `app-debug.apk` للتجربة والتثبيت المباشر.
- `app-release.apk` للتجربة كنسخة Release.

> تنبيه: نسخة Release الحالية تستخدم مفتاح Android debug لتسهيل الحصول على APK. قبل نشر التطبيق رسميًا على Google Play يجب إنشاء keystore خاص بك وتوقيع Release به، ثم حفظ بياناته كـ secrets في خدمة البناء.
