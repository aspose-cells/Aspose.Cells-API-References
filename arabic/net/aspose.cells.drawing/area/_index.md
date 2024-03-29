---
title: Area
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف الكائن الذي يمثل تنسيق المنطقة .
type: docs
weight: 1760
url: /ar/net/aspose.cells.drawing/area/
---
## Area class

لتغليف الكائن الذي يمثل تنسيق المنطقة .

```csharp
public class Area
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor) { get; set; } | الحصول على الخلفية أو تعيينهاColor التابع[`Area`](../area) . |
| [FillFormat](../../aspose.cells.drawing/area/fillformat) { get; } | يمثل أ الكائن الذي يحتوي على خصائص تنسيق التعبئة للشكل أو الرسم البياني المحدد. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor) { get; set; } | الحصول على المقدمة أو تعيينهاColor . |
| [Formatting](../../aspose.cells.drawing/area/formatting) { get; set; } | يمثل تنسيق المنطقة . |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative) { get; set; } | إذا كانت الخاصية صحيحة وكانت قيمة نقطة المخطط رقمًا سالبًا ، فسيتم استبدال لون المقدمة ولون الخلفية. |
| [Transparency](../../aspose.cells.drawing/area/transparency) { get; set; } | إرجاع أو تعيين درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (واضح) . |

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
worksheet.Cells["A2"].PutValue(100);
// إضافة قيمة عينة إلى الخلية "A3"
worksheet.Cells["A3"].PutValue(150);
// إضافة قيمة عينة إلى الخلية "B1"
worksheet.Cells["B1"].PutValue(60);
// إضافة قيمة عينة إلى الخلية "B2"
worksheet.Cells["B2"].PutValue(32);
// إضافة قيمة عينة إلى الخلية "B3"
worksheet.Cells["B3"].PutValue(50);
// إضافة مخطط إلى ورقة العمل
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
// الوصول إلى مثيل المخطط المضاف حديثًا
Chart chart = worksheet.Charts[chartIndex];
// إضافة NSeries (مصدر بيانات المخطط) إلى المخطط الذي يتراوح من خلية "A1" إلى "B3"
chart.NSeries.Add("A1:B3", true);
// ضبط لون المقدمة لمنطقة المؤامرة
chart.PlotArea.Area.ForegroundColor = Color.Blue;
// تعيين لون المقدمة لمنطقة الرسم البياني
chart.ChartArea.Area.ForegroundColor = Color.Yellow;
// تعيين لون المقدمة لمنطقة سلسلة NS الأولى
chart.NSeries[0].Area.ForegroundColor = Color.Red;
// ضبط لون المقدمة لمنطقة نقطة NSeries الأولى
chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
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
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'إضافة مخطط إلى ورقة العمل
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'الوصول إلى مثيل المخطط المضاف حديثًا
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)
'ضبط لون المقدمة لمساحة الرسم
chart.PlotArea.Area.ForegroundColor = Color.Blue
'تعيين لون المقدمة لمنطقة الرسم البياني
chart.ChartArea.Area.ForegroundColor = Color.Yellow
'ضبط اللون الأمامي لمنطقة NSeries الأولى
chart.NSeries(0).Area.ForegroundColor = Color.Red
'ضبط لون المقدمة لمساحة نقطة NSeries الأولى
chart.NSeries(0).Points(0).Area.ForegroundColor = Color.Cyan
'حفظ ملف Excel
workbook.Save("book1.xls")
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
