---
title: "فئة Line"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.Line. تغلف الكائن الذي يمثل تنسيق الخط"
type: docs
url: /ar/net/aspose.cells.drawing/line/
---
## Line class

يغلف الكائن الذي يمثل تنسيق الخط.

```csharp
public class Line
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | يحدد طول رأس السهم لبداية الخط. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | يحدد عرض رأس السهم لبداية الخط. |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | يحدد رأس السهم لبداية الخط. |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | يحدد نهايات القبّعات. |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | يمثل لون الخط. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | يحدد نوع الخط المركب |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | يحدد نوع الخط المتقطع |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | يحدد طول رأس السهم لنهاية الخط. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | يحدد عرض رأس السهم لنهاية الخط. |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | يحدد رأس السهم لنهاية الخط. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | يحصل أو يضبط نوع التنسيق. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | يمثل تعبئة متدرجة. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | يشير إلى ما إذا كان نمط الخط هذا مُعينًا تلقائيًا. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | يشير إلى ما إذا كان لون الخط مُعينًا تلقائيًا. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | يمثل ما إذا كان الخط مرئيًا. |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | يحدد أغطية الانضمام. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | يمثل نمط الخط. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | يحصل على ويضبط لون السمة. |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | يحصل أو يضبط الـ[`WeightType`](../weighttype/) للخط. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | يحصل على أو يضبط وزن الخط بوحدة النقاط. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | يحصل أو يضبط وزن الخط بوحدة البكسل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cells cells = sheet.Cells;
            cells[0,1].PutValue("Income");
            cells[1,0].PutValue("Company A");
            cells[2,0].PutValue("Company B");
            cells[3,0].PutValue("Company C");
            cells[1,1].PutValue(10000);
            cells[2,1].PutValue(20000);
            cells[3,1].PutValue(30000);
            
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 9, 9, 21, 15);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            chart.NSeries.Add("B1:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            chart.NSeries[0].Border.Style = LineType.Dot;
            chart.NSeries[0].Border.Color = Color.Red;
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
            chart.NSeries[0].Border.Weight = WeightType.MediumLine;
            
            workbook.Save("LineChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


