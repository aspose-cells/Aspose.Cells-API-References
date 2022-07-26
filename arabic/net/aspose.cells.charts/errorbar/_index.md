---
title: ErrorBar
second_title: Aspose.Cells لمرجع .NET API
description: يمثل شريط خطأ لسلسلة البيانات.
type: docs
weight: 630
url: /ar/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

يمثل شريط خطأ لسلسلة البيانات.

```csharp
public class ErrorBar : Line
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | يمثل مقدار شريط الخطأ .  يجب أن يكون المبلغ أكبر من أو يساوي الصفر. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | يحدد طول رأس السهم لبداية السطر. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | يحدد عرض رأس السهم لبداية السطر. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | يحدد رأس سهم لبداية السطر. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | يحدد سقف النهاية. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | يمثل ملفColor من الخط . |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | يحدد نوع الخط المركب |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | يحدد نوع خط الشرطة |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | يمثل نوع عرض شريط الخطأ. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | يحدد طول رأس السهم لنهاية السطر. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | يحدد عرض رأس السهم لنهاية السطر. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | يحدد رأس سهم لنهاية السطر. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | الحصول على نوع التنسيق أو تعيينه. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | يمثل تعبئة متدرجة . |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | يشير إلى ما إذا تم تعيين نمط الخط هذا تلقائيًا. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | يشير إلى ما إذا كان لون الخط معينًا تلقائيًا. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | يمثل ما إذا كان الخط مرئيًا. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | يحدد أغطية الانضمام . |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | يمثل مقدار الخطأ السالب عندما يكون نوع شريط الخطأ مخصص. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | يمثل مقدار الخطأ الإيجابي عندما يكون نوع شريط الخطأ مخصص. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | يشير إلى ما إذا كان تنسيق أشرطة الخطأ باستخدام T-top . |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | يمثل نمط الخط . |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | الحصول على لون المظهر وتعيينه. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | إرجاع أو تعيين درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (واضح) . |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | يمثل نوع مقدار شريط الخطأ. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | يحصل أو يحدد ملف[`WeightType`](../../aspose.cells.drawing/weighttype) من الخط . |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | الحصول على أو تحديد وزن الخط بوحدة النقاط. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | الحصول على أو تحديد وزن الخط بوحدة البكسل. |

### أمثلة

```csharp
[C#]
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["a1"].PutValue(2);
cells["a2"].PutValue(5);
cells["a3"].PutValue(3);
cells["a4"].PutValue(6);
cells["b1"].PutValue(4);
cells["b2"].PutValue(3);
cells["b3"].PutValue(6);
cells["b4"].PutValue(7);

cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");

int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);

Chart chart = excel.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);

chart.NSeries.CategoryData = "C1:C4";

for(int i = 0; i < chart.NSeries.Count; i ++)
{
	ASeries aseries = chart.NSeries[i];
	aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
	aseries.YErrorBar.Type = ErrorBarType.FixedValue;
	aseries.YErrorBar.Amount = 5;
}

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
Dim cells As Cells =  workbook.Worksheets(0).Cells 
cells("a1").PutValue(2)
cells("a2").PutValue(5)
cells("a3").PutValue(3)
cells("a4").PutValue(6)
cells("b1").PutValue(4)
cells("b2").PutValue(3)
cells("b3").PutValue(6)
cells("b4").PutValue(7)

cells("C1").PutValue("Q1")
cells("C2").PutValue("Q2")
cells("C3").PutValue("Y1")
cells("C4").PutValue("Y2")

Dim chartIndex As Integer =  excel.Worksheets(0).Charts.Add(ChartType.Column,11,0,27,10) 

Dim chart As Chart =  excel.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:B4", True)

chart.NSeries.CategoryData = "C1:C4"

Dim i As Integer
For  i = 0 To chart.NSeries.Count - 1
Dim aseries As ASeries =  chart.NSeries(i) 
aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus
aseries.YErrorBar.Type = ErrorBarType.FixedValue
aseries.YErrorBar.Amount = 5
Next
```

### أنظر أيضا

* class [Line](../../aspose.cells.drawing/line)
* مساحة الاسم [Aspose.Cells.Charts](../../aspose.cells.charts)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
