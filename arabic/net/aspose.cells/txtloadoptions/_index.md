---
title: TxtLoadOptions
second_title: Aspose.Cells لمرجع .NET API
description: يمثل خيارات تحميل ملف نصي.
type: docs
weight: 6110
url: /ar/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

يمثل خيارات تحميل ملف نصي.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [TxtLoadOptions](txtloadoptions#constructor)() | ينشئ خيارات تحميل ملف نصي. |
| [TxtLoadOptions](txtloadoptions#constructor_1)(LoadFormat) | ينشئ خيارات تحميل ملف نصي. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | يشير إلى ما إذا كانت التصفية التلقائية للبيانات عند تحميل الملفات. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | الحصول على خيارات التركيب التلقائي وتعيينها |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف النموذج . |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | ما إذا كان التحقق من تقييد ملف Excel عند قيام المستخدم بتعديل الكائنات ذات الصلة بالخلايا. على سبيل المثال ، لا يسمح Excel بإدخال قيمة سلسلة أطول من 32 كيلو بايت . عند إدخال قيمة أطول من 32 كيلو بايت مثل عن طريق Cell.PutValue (سلسلة) ، إذا كان هذا الخاصية صحيحة ، ستحصل على استثناء . إذا كانت هذه الخاصية خاطئة ، فسنقبل قيمة سلسلة الإدخال كقيمة للخلية بحيث يمكنك لاحقًا إخراج قيمة السلسلة الكاملة لتنسيقات الملفات الأخرى مثل CSV. ومع ذلك ، إذا لقد قمت بتعيين مثل هذا النوع من القيمة غير الصالحة لتنسيق ملف Excel ، يجب ألا تحفظ المصنف بتنسيق ملف excel لاحقًا. وإلا فقد يكون هناك خطأ غير متوقع لملف Excel الذي تم إنشاؤه. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت السلسلة في الملف النصي قد تم تحويلها إلى بيانات التاريخ. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت السلسلة في ملف نصي قد تم تحويلها إلى بيانات رقمية. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | الحصول على أو تعيين معلومات ثقافة النظام في وقت تحميل الملف. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | الحصول على إعدادات النمط الافتراضية لتهيئة أنماط المصنف |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | الحصول على الترميز الافتراضي وتعيينه. ينطبق فقط على ملف csv. |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet) { get; set; } | ما إذا كان يوسع البيانات إلى الورقة التالية عندما تتجاوز صفوف أو أعمدة البيانات الحد. إذا كانت هذه الخاصية صحيحة ، فسيتم تمديد البيانات الإضافية إلى الورقة التالية خلف الورقة الحالية (إذا كانت الورقة الحالية هي الأخيرة ، فسيتم إلحاق ورقة جديدة إلى المصنف الحالي) . إذا كانت هذه الخاصية خاطئة ، فسيتم تجاهل البيانات التي تتجاوز الحد. الافتراضي هو خطأ ؛ |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | الحصول على وتعيين تكوينات الخط الفردية. يعمل فقط مع[`Workbook`](../workbook) الذي يستخدم هذا[`LoadOptions`](../loadoptions) للتحميل.&gt; |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula) { get; set; } | يشير إلى ما إذا كان النص صيغة إذا كان يبدأ بـ "=". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier) { get; set; } | ما إذا كان هناك مؤهل نص لقيمة الخلية. الافتراضي هو الصحيح. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | تجاهل البيانات التي لم تتم طباعتها في حالة طباعة الملف مباشرة |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | الحصول على شاشة المقاطعة وتعيينها. |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded) { get; set; } | صحيح يعني أن الملف يحتوي على عدة ترميزات. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | يشير إلى ما إذا كان لا يتم تحليل قيمة سلسلة إذا كان الطول 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | ما إذا كان سيتم الاحتفاظ بالبيانات التي لم يتم تحليلها في الذاكرة للمصنف عند تحميله من ملف القالب. الافتراضي هو الصحيح. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | الحصول على أو تعيين لغة واجهة المستخدم لإصدار المصنف بناءً على كود البلد الذي حفظ الملف. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | عامل التصفية للإشارة إلى كيفية تحميل البيانات. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | يحصل على تنسيق التحميل. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | تشير إلى إستراتيجية تطبيق النمط للقيم التي تم تحليلها عند تحويل قيمة السلسلة إلى رقم أو تاريخ ووقت. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | الحصول على أو تعيين خيارات استخدام الذاكرة. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | يشير إلى ما إذا كان تحليل الصيغة عند قراءة الملف. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | يشير إلى ما إذا كان تحليل السجلات المحورية المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false . |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | الحصول على كلمة مرور المصنف وتعيينها. |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers) { get; set; } | الحصول على وتعيين محللات القيمة المفضلة لتحميل ملف نصي. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | الحصول على أو تعيين الإعدادات الإقليمية للنظام بناءً على رمز البلد في وقت تحميل الملف. |
| [Separator](../../aspose.cells/txtloadoptions/separator) { get; set; } | الحصول على وتعيين فاصل الأحرف لملف نصي. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring) { get; set; } | الحصول على قيمة سلسلة وتعيينها كفاصل . |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier) { get; set; } | تحديد مؤهل النص لقيم الخلية. المؤهل الافتراضي هو "" . |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone) { get; set; } | ما إذا كان يجب معاملة المحددات المتتالية على أنها واحدة. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue) { get; set; } | يشير إلى ما إذا كان يجب أخذ علامة الاقتباس المفردة البادئة كجزء من قيمة خلية واحدة. القيمة الافتراضية صحيحة. إذا كانت خاطئة ، فستتم إزالة علامة الاقتباس المفردة البادئة من value للخلية المقابلة و[`QuotePrefix`](../style/quoteprefix) سيتم تعيينه على أنه صحيح للخلية. |
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
