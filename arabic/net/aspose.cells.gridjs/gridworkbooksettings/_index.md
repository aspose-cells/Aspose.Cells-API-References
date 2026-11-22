---
title: "الفئة GridWorkbookSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridJs.GridWorkbookSettings. تمثل إعدادات دفتر العمل"
type: docs
url: /ar/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

يمثل إعدادات دفتر العمل.

```csharp
public class GridWorkbookSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | يحصل/يضبط مؤلف الملف. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | يشير إلى ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom، القيمة الافتراضية هي false. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على استثناء. إذا كانت false، سنقبل قيمة النص المدخلة كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة لتنسيقات ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ دفتر العمل بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. القيمة الافتراضية هي false. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | يشير إلى ما إذا كان يتم إنشاء سلسلة الصيغ المحسوبة. القيمة الافتراضية هي false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | يحصل أو يعيّن قيمة تمثل ما إذا كان المصنف يستخدم نظام التاريخ 1904. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة أخرى في دفتر العمل. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | يشير إلى ما إذا كان يتم حساب كامل في كل مرة يتم فيها تشغيل عملية حساب. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | يشير إلى ما إذا كان يتم استخدام التكرار لحل المراجع الدائرية. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | يعيد أو يضبط الحد الأقصى لعدد التكرارات لحل مرجع دائري، القيمة الافتراضية هي 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما هي معروضة |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | يشير إلى ما إذا كان يتم إعادة حساب جميع الصيغ عند فتح الملف. القيمة الافتراضية هي true. |

### أمثلة

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//قم بأعمالك

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


