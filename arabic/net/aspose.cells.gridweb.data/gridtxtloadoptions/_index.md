---
title: "الفئة GridTxtLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Data.GridTxtLoadOptions. تمثل الخيارات لتحميل ملف نصي"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

يمثل الخيارات لتحميل ملف نصي.

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | ينشئ الخيارات لتحميل ملف نصي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف القالب. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تدخل قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على استثناء. إذا كانت false، سنقبل قيمة النص التي أدخلتها كقيمة للخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة لتنسيقات ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يُحوَّل إلى بيانات تاريخ. |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان النص في ملف النص يُحوَّل إلى بيانات رقمية. |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | يحصل ويعيّن الترميز الافتراضي. ينطبق فقط على ملفات csv. |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | ما إذا كان يتم تمديد البيانات إلى الورقة التالية عندما تتجاوز الصفوف أو الأعمدة الحد. إذا كانت هذه الخاصية true، سيتم تمديد البيانات الإضافية إلى الورقة التالية خلف الحالية (إذا كانت الورقة الحالية هي الأخيرة، ستُضاف ورقة جديدة إلى المصنف الحالي). إذا كانت false، سيتم تجاهل البيانات التي تتجاوز الحد. القيمة الافتراضية هي false؛ |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=". |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | ما إذا كان هناك محدد نص لقيمة الخلية. القيمة الافتراضية هي true. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرة (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | True يعني أن الملف يحتوي على عدة ترميزات. |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | يشير إلى عدم تحليل قيمة النص إذا كان طولها 15. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | ما إذا كان يتم الاحتفاظ بالبيانات غير المُحلَّلة في الذاكرة للمصنف عند تحميله من ملف القالب. القيمة الافتراضية هي true. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف التي لم يتم تخصيصها فقط. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | يشير إلى ما إذا كان يتم تحليل الصيغة عند قراءة الملف. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | يشير إلى ما إذا كان يتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | يحصل ويعيّن كلمة مرور المصنف. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | يشير إلى ما إذا كان يتم الحفاظ على تلك المسافات وفواصل الأسطر التي تم إضافتها بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false. (موروث من [`GridLoadOptions`](../gridloadoptions/).) |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | يحصل على ويضبط فاصل الأحرف لملف النص. |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | يحصل على ويضبط قيمة سلسلة كفاصل. |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | يحدد محدد النص لقيم الخلايا. المحدد الافتراضي هو '\"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | ما إذا كان يجب معالجة الفواصل المتتالية كواحدة. |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | يشير إلى ما إذا كان يجب اعتبار علامة الاقتباس المفردة الأولية جزءًا من قيمة الخلية. القيمة الافتراضية هي true. إذا كانت false، سيتم إزالة علامة الاقتباس المفردة الأولية من قيمة الخلية المقابلة وسيتم تعيين [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) إلى true للخلية. |

### انظر أيضًا

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


