---
title: ChartArea
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف الكائن الذي يمثل منطقة المخطط في ورقة العمل.
type: docs
weight: 440
url: /ar/net/aspose.cells.charts/chartarea/
---
## ChartArea class

لتغليف الكائن الذي يمثل منطقة المخطط في ورقة العمل.

```csharp
public class ChartArea : ChartFrame
```

## الخصائص

| اسم | وصف |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | يحصل على ملف[`منطقة`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True إذا كان النص الموجود في الكائن يغير حجم الخط عندما يتغير حجم الكائن. القيمة الافتراضية هي الحقيقية. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | الحصول على وضبط وضع عرض الخلفية |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | يحصل على ملف[`الحدود`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | يمثل ارتفاع الموضع الافتراضي |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | يمثل عرض الموضع الافتراضي |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | يمثل x الوضع الافتراضي |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | يمثل y الوضع الافتراضي |
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | يحصل على أ[`Font`](./font) كائن من كائن المخطط المحدد . |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | الحصول على أو تعيين الإزاحة الرأسية من صف الزاوية اليمنى السفلي. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | يشير إلى ما إذا كان حجم إطار المخطط تلقائيًا. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | يشير إلى ما إذا كان قد تم تعيين الموضع الافتراضي (الافتراضي X ، الافتراضي Y ، العرض الافتراضي والارتفاع الافتراضي). |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | يشير إلى ما إذا كان حجم مساحة قطعة الأرض يتضمن علامات التجزئة ، وتسميات المحور. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | صحيح إذا كان للإطار ظل. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | يحصل على ملف[`ShapeProperties`](../chartframe/shapeproperties) الكائن . |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | الحصول على أو تعيين الإزاحة الأفقية من عمود الزاوية اليمنى السفلي. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | الحصول على أو الحصول على الإزاحة الأفقية من عمود الزاوية اليسرى العليا. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | الحصول على أو الحصول على الإزاحة الرأسية من صف الزاوية اليسرى العليا. |

## طُرق

| اسم | وصف |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | ضبط موضع الإطار على Automatic |

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();

// الحصول على مرجع ورقة العمل الأولى
Worksheet worksheet = workbook.Worksheets[0];

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

// الحصول على منطقة المخطط
ChartArea chartArea = chart.ChartArea;

// تعيين لون المقدمة لمنطقة الرسم البياني
chartArea.Area.ForegroundColor = Color.Yellow;

// إعداد ظل منطقة الرسم البياني
chartArea.Shadow = true;

// حفظ ملف Excel
workbook.Save("book1.xls");

[VB.NET]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()

'الحصول على مرجع ورقة العمل الأولى
Dim worksheet As Worksheet = workbook.Worksheets(0)

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

'الحصول على منطقة المخطط
Dim chartArea As ChartArea = chart.ChartArea

'تعيين لون المقدمة لمنطقة الرسم البياني
chartArea.Area.ForegroundColor = Color.Yellow

'إعداد ظل منطقة المخطط
chartArea.Shadow = True

'حفظ ملف Excel
workbook.Save("book1.xls")
```

### أنظر أيضا

* class [ChartFrame](../chartframe)
* مساحة الاسم [Aspose.Cells.Charts](../../aspose.cells.charts)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
