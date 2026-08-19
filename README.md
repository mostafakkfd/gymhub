# GymHub — نظام إدارة الأندية والجيمات

## هيكل المشروع

```
GymHub/
├── dashboard/                 ← المنتج الرئيسي (الداشبورد)
│   ├── index.html             لوحة التحكم (تسجيل دخول + إدارة المشتركين/الاشتراكات/التقارير)
│   ├── style.css              هوية الداشبورد (بهوية اللاندنج: كحلي/برتقالي/أخضر)
│   ├── app.bundle.js          منطق التطبيق (Supabase)
│   ├── gymhub-logo.png        شعار البراند الشفاف
│   ├── favicon-32x32.png
│   └── apple-touch-icon.png
│
├── landing/                   ← صفحة الهبوط التسويقية
│   ├── index.html             اللاندنج الكامل (hero + مميزات + أسعار + تواصل)
│   ├── assets/logo.png        شعار البراند
│   ├── dashboard-dark.png     لقطة الداشبورد (ثيم داكن)
│   ├── dashboard-light.png    لقطة الداشبورد (ثيم فاتح)
│   ├── dashboard-mobile-dark.png   لقطة الهاتف (ثيم داكن)
│   ├── dashboard-mobile-light.png  لقطة الهاتف (ثيم فاتح)
│   └── previews/              أرشيف لقطات قديمة
│
└── README.md
```

## ملاحظات
- الثيم موحّد بين اللاندنج والداشبورد عبر مفتاح `gymhub-theme` في localStorage.
- صور الهاتف في اللاندنج تتبدل تلقائياً حسب ثيم الموقع (داكن → فاتحة، فاتح → داكنة).
- الداشبورد يتصل بـ Supabase (anon key داخل `app.bundle.js`).
