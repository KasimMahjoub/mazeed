# Mazeed: mazeed.com.ly

موقع مزيد للأبحاث والتدريب، بتبويبين: مزيد و دُوري.
عربي وإنجليزي، فاتح وداكن، خط Janna فقط.

## الملفات
```
index.html              الصفحة كاملة (لا تحتاج أي مكتبة خارجية)
assets/janna.woff       خط Janna (الأساسي)
assets/janna.ttf        خط Janna (احتياطي)
assets/mazeed-logo.png  الشعار
CNAME                   ربط النطاق mazeed.com.ly
README.md               هذا الملف
```

## النشر على GitHub Pages
1. أنشئ مستودعًا جديدًا (مثلًا: mazeed) وارفع الملفات كما هي إلى الجذر، مع مجلد assets.
2. Settings ثم Pages: Deploy from a branch، الفرع main، المجلد / (root).
3. Custom domain: اكتب mazeed.com.ly ثم Save.

## سجلات DNS في ليبيان سبايدر (DNS Manager ثم Add Record)

| النوع | الاسم | القيمة |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | kasimmahjoub.github.io |
| CNAME | duri | kasimmahjoub.github.io |

- سجل duri موجود مسبقًا، اتركه كما هو (يخدم مستودع duri4).
- إذا وُجدت سجلات A قديمة على @ تشير لاستضافة ليبيان سبايدر، احذفها.
- الانتشار يأخذ من دقائق إلى 24 ساعة. بعدها فعّل Enforce HTTPS من صفحة Pages.

## تعديل الروابط
في أعلى السكربت داخل index.html:
```
var LINKS={survey:'https://kasimmahjoub.github.io/duri4/', results:'https://kasimmahjoub.github.io/duri4/results/', page:'https://mazeed.com.ly/#duri'};
```
عندما يعمل duri.mazeed.com.ly غيّر أول رابطين إلى:
`https://duri.mazeed.com.ly/` و `https://duri.mazeed.com.ly/results/`

## روابط مباشرة
- mazeed.com.ly يفتح تبويب مزيد
- mazeed.com.ly/#duri يفتح تبويب دُوري
