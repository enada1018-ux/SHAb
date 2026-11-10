# بوابة حجز ودفع المصروفات - أكاديمية الشروق

صفحة تجريبية لحجز المواعيد ودفع المصروفات. كل البيانات والمدفوعات فيها تجريبية ومش مربوطة بنظام الأكاديمية ولا ببوابة دفع، ومفيش أي فلوس بتتخصم.

## الملفات

```
shorouk-portal/
├── index.html      الصفحة
├── style.css       التصميم
├── app.js          الكود (الحجز، الدفع، اللغة، الوضع الليلي)
└── assets/
    ├── logo.jpg    شعار الأكاديمية
    └── campus.jpg  صورة الهيرو
```

## الفتح من VS Code

1. افتح VS Code، ثم File > Open Folder واختار مجلد `shorouk-portal`.
2. ثبّت إضافة **Live Server**، ثم كليك يمين على `index.html` واختار **Open with Live Server**.
3. ولو عاوز بس تشوفها، افتح `index.html` بدبل كليك في المتصفح.

لتنسيق الكود لو عاوز تقرأه بسهولة: افتح الملف واضغط `Shift + Alt + F`.

## الرفع على GitHub

1. أنشئ Repository جديد على GitHub باسم `shorouk-portal` (من غير README).
2. من التيرمنال جوه المجلد:

```bash
git init
git add .
git commit -m "Shorouk portal"
git branch -M main
git remote add origin https://github.com/USERNAME/shorouk-portal.git
git push -u origin main
```

(بدّل `USERNAME` باسم حسابك.) أو ارفع الملفات من زر **Add file > Upload files** في GitHub.

## نشرها كموقع (GitHub Pages)

1. في الـ Repository: **Settings > Pages**.
2. في **Source** اختار **Deploy from a branch**، والفرع `main` والمجلد `/ (root)`، ثم **Save**.
3. بعد دقيقة أو اتنين الرابط هيكون:
   `https://USERNAME.github.io/shorouk-portal/`

## تعديلات سريعة

- **صورة الهيرو أو الشعار:** استبدل الملف في `assets/` بنفس الاسم.
- **بنود المصروفات والمبالغ:** في `index.html` ابحث عن `id="fee"`.
- **حجوزات ومدفوعات البداية:** في `app.js` ابحث عن `fresh=`.
