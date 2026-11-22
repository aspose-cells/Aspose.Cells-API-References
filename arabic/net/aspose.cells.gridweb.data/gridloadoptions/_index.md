---
title: "فئة GridLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridWeb.Data.GridLoadOptions. تمثل خيارات تحميل الملف. قديمة هذا الفئة ستصبح مهجورة بعد استخدام DLL مستقل لواجهة برمجة تطبيقات الخلايا العامة، بدلاً من ذلك يمكنك استخدام Aspose.Cells.LodOptions"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridloadoptions/
---
## GridLoadOptions class

يمثل خيارات تحميل الملف. [Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions ")]

```csharp
public class GridLoadOptions : ISerializable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridLoadOptions](gridloadoptions/)() | إنشاء خيارات تحميل الملف. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | يشير إلى ما إذا كان يتم تصفية البيانات تلقائيًا عند تحميل الملفات. |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | تحقق مما إذا كانت البيانات صالحة في ملف القالب. |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على استثناء. إذا كانت false، سنقبل قيمة النص المدخلة كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة إلى صيغ ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | تجاهل البيانات التي لا تُطبع إذا تم طباعة الملف مباشرةً |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | ما إذا كان سيتم الاحتفاظ بالبيانات غير المُحللة في الذاكرة لدفتر العمل عندما يتم تحميله من ملف القالب. القيمة الافتراضية هي true. |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | يوضح ما إذا كان يتم ضبط الصفوف فقط التي ليس ارتفاعها مخصصًا. |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | يشير إلى ما إذا كان سيتم تحليل الصيغة عند قراءة الملف. |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | يشير إلى ما إذا كان سيتم تحليل سجلات Pivot المخزنة مؤقتًا عند تحميل الملف. القيمة الافتراضية هي false. |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | يحصل على ويضبط كلمة مرور دفتر العمل. |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | يشير إلى ما إذا كان سيتم الحفاظ على تلك الفراغات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وضبطها. القيمة الافتراضية هي false. |

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


