---
title: FillFormat
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف الكائن الذي يمثل تنسيق التعبئة لشكل.
type: docs
weight: 1970
url: /ar/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

لتغليف الكائن الذي يمثل تنسيق التعبئة لشكل.

```csharp
public class FillFormat
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | الحصول على نوع التعبئة وتعيينه |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | إرجاع لون التدرج 1 للتعبئة المحددة. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | إرجاع لون التدرج 2 للتعبئة المحددة. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | إرجاع نوع لون التدرج للتعبئة المحددة. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | إرجاع درجة التدرج للتعبئة المحددة. ينطبق فقط على Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | يحصل[`GradientFill`](./gradientfill) الكائن . |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | إرجاع نمط التدرج للتعبئة المحددة. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | إرجاع متغير التدرج للتعبئة المحددة. ينطبق فقط على Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | الحصول على بيانات صورة الصورة وتعيينها. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | يمثل نمط عرض منطقة . |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | يحصل[`PatternFill`](./patternfill) الكائن . |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | الحصول على نوع تنسيق الصورة وتعيينه. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | إرجاع لون التدرج المحدد مسبقًا للتعبئة المحددة. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | الحصول على مقياس تنسيق الصورة وتعيينه . |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | يحصل[`SolidFill`](./solidfill) الكائن . |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | يمثل نوع النسيج للتعبئة المحددة. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | يحصل[`TextureFill`](./texturefill) الكائن . |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | إرجاع أو تعيين درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (واضح) . |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | يحصل على كود التجزئة . |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | يعين التعبئة المحددة إلى تدرج أحادي اللون. ينطبق فقط على Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | تعيين التعبئة المحددة لتدرج لوني محدد مسبقًا. ينطبق فقط على Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | يعين التعبئة المحددة إلى تدرج لوني ثنائي اللون. ينطبق فقط على Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | يعين التعبئة المحددة إلى تدرج لوني ثنائي اللون. ينطبق فقط على Excel 2007. |

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();
// إضافة ورقة عمل جديدة إلى كائن Excel
int sheetIndex = workbook.Worksheets.Add();
// الحصول على مرجع ورقة العمل المضافة حديثًا عن طريق تمرير فهرس الورقة الخاص بها
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// إضافة قيمة عينة إلى الخلية "A1"
worksheet.Cells["A1"].PutValue(50);
// إضافة قيمة عينة إلى الخلية "A2"
worksheet.Cells["A2"].PutValue(100);
// إضافة قيمة عينة إلى الخلية "A3"
worksheet.Cells["A3"].PutValue(150);
// إضافة قيمة عينة إلى الخلية "A4"
worksheet.Cells["A4"].PutValue(200);
// إضافة قيمة عينة إلى الخلية "B1"
worksheet.Cells["B1"].PutValue(60);
// إضافة قيمة عينة إلى الخلية "B2"
worksheet.Cells["B2"].PutValue(32);
// إضافة قيمة عينة إلى الخلية "B3"
worksheet.Cells["B3"].PutValue(50);
// إضافة قيمة عينة إلى الخلية "B4"
worksheet.Cells["B4"].PutValue(40);
// إضافة قيمة عينة إلى خلية "C1" كبيانات فئة
worksheet.Cells["C1"].PutValue("Q1");
// إضافة قيمة عينة إلى خلية "C2" كبيانات فئة
worksheet.Cells["C2"].PutValue("Q2");
// إضافة قيمة عينة إلى خلية "C3" كبيانات فئة
worksheet.Cells["C3"].PutValue("Y1");
// إضافة قيمة عينة إلى خلية "C4" كبيانات فئة
worksheet.Cells["C4"].PutValue("Y2");
// إضافة مخطط إلى ورقة العمل
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
// الوصول إلى مثيل المخطط المضاف حديثًا
Chart chart = worksheet.Charts[chartIndex];
// إضافة NSeries (مصدر بيانات المخطط) إلى المخطط الذي يتراوح من خلية "A1" إلى "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
// تعيين مصدر البيانات لبيانات فئة سلسلة NS
chart.NSeries.CategoryData = "C1:C4";
// ملء مساحة سلسلة NS الثانية بتدرج لوني
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()
'إضافة ورقة عمل جديدة إلى كائن Excel
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'الحصول على مرجع ورقة العمل المضافة حديثًا عن طريق تمرير فهرس الورقة الخاص بها
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'إضافة مخطط إلى ورقة العمل
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'الوصول إلى مثيل المخطط المضاف حديثًا
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'ضبط مصدر البيانات لبيانات فئة NSeries
chart.NSeries.CategoryData = "C1:C4"
'ملء مساحة سلسلة NS الثانية بتدرج لوني
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
