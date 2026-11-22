---
title: "الفئة GridWorkbookSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Data.GridWorkbookSettings. تمثل إعدادات دفتر العمل"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

يمثل إعدادات المصنف.

```csharp
public class GridWorkbookSettings : ISerializable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | منشئ افتراضي |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | يحصل على مؤلف الملف ويضبطه. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | يحصل أو يحدد ما إذا كان يتم فحص تنسيق الرقم المخصص عند تعيين Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | يحصل أو يحدد ما إذا كان يتم إنشاء سلسلة صيغ محسوبة. القيمة الافتراضية هي false. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | يحصل أو يحدد القيمة التي تمثل ما إذا كان المصنف يستخدم نظام التاريخ 1904. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | يحصل أو يحدد ما إذا كان تمكين الماكرو؛ الآن يعمل فقط عند نسخ ورقة عمل إلى ورقة عمل أخرى في المصنف. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | يحصل أو يحدد ما إذا كان يتم حساب كامل في كل مرة يتم فيها تشغيل عملية حساب. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | يحصل أو يحدد ما إذا كان يتم استخدام التكرار لحل الإشارات الدائرية. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | يحصل أو يحدد الحد الأقصى لعدد التكرارات لحل إشارة دائرية، القيمة الافتراضية هي 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | صحيح إذا كانت الحسابات في هذا المصنف ستُجرى باستخدام دقة الأرقام كما هي معروضة |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | يشير إلى ما إذا كان سيتم الحفاظ على تلك الفراغات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وضبطها. القيمة الافتراضية هي false. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | يحصل أو يحدد ما إذا كان يتم إعادة حساب جميع الصيغ عند فتح الملف. |

### أمثلة

```csharp
[C#]

 
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//قم بأعمالك

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb.Settings=gsettings;
 
'do your business
```

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


