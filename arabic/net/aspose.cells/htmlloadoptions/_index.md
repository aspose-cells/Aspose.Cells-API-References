---
title: HtmlLoadOptions
second_title: Aspose.Cells لمرجع .NET API
description: يمثل خيارات عند استيراد ملف html.
type: docs
weight: 3730
url: /ar/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

يمثل خيارات عند استيراد ملف html.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions#constructor)() | ينشئ خيارات لتحميل الملف. |
| [HtmlLoadOptions](htmlloadoptions#constructor_1)(LoadFormat) | ينشئ خيارات لتحميل الملف. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | يشير إلى ما إذا كانت التصفية التلقائية للبيانات عند تحميل الملفات. |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows) { get; set; } | يشير إلى ما إذا كان يتم احتواء الأعمدة والصفوف تلقائيًا. القيمة الافتراضية هي كاذبة. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | الحصول على خيارات التركيب التلقائي وتعيينها |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف النموذج . |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | ما إذا كان التحقق من تقييد ملف Excel عند قيام المستخدم بتعديل الكائنات ذات الصلة بالخلايا. على سبيل المثال ، لا يسمح Excel بإدخال قيمة سلسلة أطول من 32 كيلو بايت . عند إدخال قيمة أطول من 32 كيلو بايت مثل عن طريق Cell.PutValue (سلسلة) ، إذا كان هذا الخاصية صحيحة ، ستحصل على استثناء . إذا كانت هذه الخاصية خاطئة ، فسنقبل قيمة سلسلة الإدخال كقيمة للخلية بحيث يمكنك لاحقًا إخراج قيمة السلسلة الكاملة لتنسيقات الملفات الأخرى مثل CSV. ومع ذلك ، إذا لقد قمت بتعيين مثل هذا النوع من القيمة غير الصالحة لتنسيق ملف Excel ، يجب ألا تحفظ المصنف بتنسيق ملف excel لاحقًا. وإلا فقد يكون هناك خطأ غير متوقع لملف Excel الذي تم إنشاؤه. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت السلسلة في الملف النصي قد تم تحويلها إلى بيانات التاريخ. |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata) { get; set; } | إذا كان صحيحًا ، فقم بتحويل السلسلة إلى صيغة عندما تبدأ قيمة السلسلة بالحرف '=' ، فالقيمة الافتراضية هي false . |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت السلسلة في ملف نصي قد تم تحويلها إلى بيانات رقمية. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | الحصول على أو تعيين معلومات ثقافة النظام في وقت تحميل الملف. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | الحصول على إعدادات النمط الافتراضية لتهيئة أنماط المصنف |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces) { get; set; } | يشير إلى ما إذا كان سيتم حذف المسافات الزائدة عندما يلتف النص على الأسطر باستخدام علامة &lt;br&gt;. القيمة الافتراضية هي false . |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | الحصول على الترميز الافتراضي وتعيينه. ينطبق فقط على ملف csv. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | الحصول على وتعيين تكوينات الخط الفردية. يعمل فقط مع[`Workbook`](../workbook) الذي يستخدم هذا[`LoadOptions`](../loadoptions) للتحميل.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | تجاهل البيانات التي لم تتم طباعتها في حالة طباعة الملف مباشرة |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | الحصول على شاشة المقاطعة وتعيينها. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | يشير إلى ما إذا كان لا يتم تحليل قيمة سلسلة إذا كان الطول 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | ما إذا كان سيتم الاحتفاظ بالبيانات التي لم يتم تحليلها في الذاكرة للمصنف عند تحميله من ملف القالب. الافتراضي هو الصحيح. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | الحصول على أو تعيين لغة واجهة المستخدم لإصدار المصنف بناءً على كود البلد الذي حفظ الملف. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | عامل التصفية للإشارة إلى كيفية تحميل البيانات. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | يحصل على تنسيق التحميل. |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas) { get; set; } | يشير إلى ما إذا كان استيراد الصيغ إذا كان ملف html الأصلي يحتوي على صيغ |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | تشير إلى إستراتيجية تطبيق النمط للقيم التي تم تحليلها عند تحويل قيمة السلسلة إلى رقم أو تاريخ ووقت. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | الحصول على أو تعيين خيارات استخدام الذاكرة. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | يشير إلى ما إذا كان تحليل الصيغة عند قراءة الملف. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | يشير إلى ما إذا كان تحليل السجلات المحورية المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false . |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | الحصول على كلمة مرور المصنف وتعيينها. |
| [ProgId](../../aspose.cells/htmlloadoptions/progid) { get; } | يحصل على معرف البرنامج الخاص بإنشاء الملف. لملفات MHT فقط. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | الحصول على أو تعيين الإعدادات الإقليمية للنظام بناءً على رمز البلد في وقت تحميل الملف. |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider) { get; set; } | الحصول على أو تعيين StreamProviderImportHtmlFile لاستيراد الكائنات. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag) { get; set; } | يشير إلى ما إذا كان يدعم تخطيط علامة &lt;div&gt; عندما يحتوي ملف html على علامات &lt;div&gt;. القيمة الافتراضية هي كاذبة. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | الحصول على رد اتصال التحذير أو تعيينه . |

## طُرق

| اسم | وصف |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | يعين حجم ورق الطباعة الافتراضي من إعداد الطابعة الافتراضية. |

### أنظر أيضا

* class [AbstractTextLoadOptions](../abstracttextloadoptions)
* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
