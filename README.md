# Mazeed: mazeed.com.ly

موقع مزيد للأبحاث والتدريب: صفحة واحدة، مع تسجيل الاهتمام وترشيح الطلبة عبر واتساب.
عربي وإنجليزي، فاتح وداكن، خط Janna فقط.

## الملفات
```
index.html              الصفحة كاملة (لا تحتاج أي مكتبة خارجية)
assets/janna.woff       خط Janna (الأساسي)
assets/janna.ttf        خط Janna (احتياطي)
assets/mazeed-logo.png  الشعار
assets/mazeed-logo-light.png  الشعار للوضع الداكن
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

## تعديل الرقم والروابط
في أعلى السكربت داخل index.html:
```
var CONTACT={ whatsapp:'218927678699', email:'info@mazeed.com.ly' };
var LINKS={ survey:'https://kasimmahjoub.github.io/duri4/', results:'https://kasimmahjoub.github.io/duri4/results/', site:'https://mazeed.com.ly/#register' };
```
عندما يعمل duri.mazeed.com.ly غيّر أول رابطين إلى:
`https://duri.mazeed.com.ly/` و `https://duri.mazeed.com.ly/results/`

## روابط مباشرة
- mazeed.com.ly/#register يفتح نموذج التسجيل
- mazeed.com.ly/#refer يفتح نموذج ترشيح طالب
