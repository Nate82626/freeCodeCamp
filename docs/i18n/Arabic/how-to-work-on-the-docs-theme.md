# كيفية العمل في موضوع الوثائق

> [!ملاحظة] تذكير سريع بأنك لست بحاجة إلى إعداد أي شيء للعمل على محتوى موقع التوثيق.
> 
> للعمل على المبادئ التوجيهية للمساهمة، يمكنك تعديل أو إضافة ملفات في دليل `docs` [المتاح هنا](https://github.com/freeCodeCamp/freeCodeCamp/tree/master/docs). عند دمج التغييرات الخاصة بك، سيتم إتاحتها تلقائياً في موقع التوثيق.

## هيكل موقع الوثائق على الإنترنت

تم إنشاء الموقع باستخدام [`docsify`](https://docsify.js.org)، وتم خدمته باستخدام صفحات GitHub .

عادة لن تحتاج إلى تغيير أي تكوين أو بناء الموقع محليا. في حالة إهتمامك، إليك كيفية عملها:

- مصدر الصفحة الرئيسية لهذا الموقع متاح في [`docs/index.html`](index.html).
- نحن نخدم هذا الملف كـ SPA باستخدام `docsify` وصفحات GitHub .
- البرنامج النصي `docsify` يولد محتوى `markdown` ملفات في `docs` دليل عند الطلب.
- تم إنشاء الصفحة الرئيسية من [`_coverpage.md`](_coverpage.md).
- التنقل في الشريط الجانبي يتم إنشاؤه من [`_sidebar.md`](_sidebar.md).

## تقديم الخدمات لموقع الوثائق محليا

استنساخ معسكر الترميز الحر:

```sh
استنساخ git https://github.com/freeCodeCamp/freeCodeCamp.git
docsify يخدم المستندات
```

تثبيت `docsify`:

```sh
npm install -g docsify
```

وخدمة دليل `/docs`

```sh
docsify يخدم المستندات
```

بدلاً من ذلك، إذا كنت قد قمت بتثبيت freeCodeCamp محلياً (انظر دليل الإعداد المحلي)، نقوم بتجميع CLI مع أدوات التطوير حتى يمكنك تشغيل `npm تشغيل docs:serve` من جذر المستودع.
