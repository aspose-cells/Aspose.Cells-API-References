---
title: InvertIfNegative
second_title: Aspose.Cells لمرجع .NET API
description: إذا كانت الخاصية صحيحة وكانت قيمة نقطة المخطط رقمًا سالبًا  فسيتم استبدال لون المقدمة ولون الخلفية.
type: docs
weight: 50
url: /ar/net/aspose.cells.drawing/area/invertifnegative/
---
## Area.InvertIfNegative property

إذا كانت الخاصية صحيحة وكانت قيمة نقطة المخطط رقمًا سالبًا ، فسيتم استبدال لون المقدمة ولون الخلفية.

```csharp
public bool InvertIfNegative { get; set; }
```

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();
// إضافة ورقة عمل جديدة إلى كائن المصنف
int sheetIndex = workbook.Worksheets.Add();
// الحصول على مرجع ورقة العمل المضافة حديثًا عن طريق تمرير فهرس الورقة الخاص بها
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// إضافة قيمة عينة إلى الخلية "A1"
worksheet.Cells["A1"].PutValue(50);
// إضافة قيمة عينة إلى الخلية "A2"
worksheet.Cells["A2"].PutValue(-100);
// إضافة قيمة عينة إلى الخلية "A3"
worksheet.Cells["A3"].PutValue(150);
// إضافة مخطط إلى ورقة العمل
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
// الوصول إلى مثيل المخطط المضاف حديثًا
Chart chart = worksheet.Charts[chartIndex];
// إضافة NSeries (مصدر بيانات المخطط) إلى المخطط الذي يتراوح من خلية "A1" إلى "A3"
chart.NSeries.Add("A1:A3", true);
chart.NSeries[0].Area.InvertIfNegative = true;
// تعيين لون المقدمة لمنطقة سلسلة NS الأولى
chart.NSeries[0].Area.ForegroundColor = Color.Red;
// تعيين لون الخلفية لمنطقة NSeries الأولى.
// سيكون لون المنطقة المعروضة في نقطة الرسم البياني الثانية هو لون الخلفية.
chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
// حفظ ملف Excel
workbook.Save("book1.xls");

[Visual Basic]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()
'إضافة ورقة عمل جديدة إلى كائن المصنف
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'الحصول على مرجع ورقة العمل المضافة حديثًا عن طريق تمرير فهرس الورقة الخاص بها
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(-100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'إضافة مخطط إلى ورقة العمل
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'الوصول إلى مثيل المخطط المضاف حديثًا
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.NSeries.Add("A1:A3", True)
chart.NSeries(0).Area.InvertIfNegative = True
'ضبط اللون الأمامي لمنطقة NSeries الأولى
chart.NSeries(0).Area.ForegroundColor = Color.Red
'ضبط لون الخلفية لمنطقة سلسلة NS الأولى.
'سيكون لون المنطقة المعروضة في نقطة الرسم البياني الثانية هو لون الخلفية.
chart.NSeries(0).Area.BackgroundColor = Color.Yellow
'حفظ ملف Excel
workbook.Save("book1.xls")

```

### أنظر أيضا

* class [Area](../../area)
* مساحة الاسم [Aspose.Cells.Drawing](../../area)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
