# التقويم الذكي (Smart Calendar) — واجهة تجريبية

نسخة أمامية بسيطة (HTML/CSS/JS بدون أي مكتبات خارجية إلزامية) تحاكي تصميم لوحة تحكم تقويم دراسي: بطاقات إحصائيات، قائمة أسابيع دراسية، الأحداث القادمة، والفئات — بدعم كامل للغة العربية واتجاه RTL.

## الملفات
- `index.html` — الصفحة كاملة (HTML + CSS + JS مضمّنة في ملف واحد)

## التشغيل محليًا
لا حاجة لأي تثبيت. فقط افتح `index.html` في المتصفح مباشرة، أو شغّل خادمًا محليًا بسيطًا:

```bash
python3 -m http.server 8000
# ثم افتح http://localhost:8000
```

## رفع المشروع إلى GitHub

1. أنشئ مستودعًا جديدًا على GitHub (بدون README لتفادي تعارض الملفات).
2. من داخل مجلد المشروع نفّذ:

```bash
git init
git add .
git commit -m "Initial commit: Smart Calendar UI"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO_NAME.git
git push -u origin main
```

استبدل `USERNAME` و `REPO_NAME` باسم حسابك واسم المستودع.

## النشر مجانًا عبر GitHub Pages
1. في المستودع، اذهب إلى **Settings → Pages**.
2. تحت **Source** اختر الفرع `main` والمجلد `/ (root)`.
3. احفظ، وستحصل خلال دقيقة على رابط مثل:
   `https://USERNAME.github.io/REPO_NAME/`

## تعديل البيانات
كل البيانات (الأحداث، الأسابيع، الفئات، الإحصائيات) موجودة في متغيرات JavaScript أعلى نهاية ملف `index.html` (`stats`, `categories`, `weeks`, `upcoming`) — عدّلها مباشرة لتغيير المحتوى المعروض.

## ملاحظة
هذا التصميم مستوحى من واجهة تطبيق تقويم دراسي، وهو تصميم مبسّط للتوضيح والانطلاق منه — يمكنك تطويره لاحقًا بربطه بقاعدة بيانات حقيقية (مثل Supabase أو Firebase) بدلاً من البيانات الثابتة.
