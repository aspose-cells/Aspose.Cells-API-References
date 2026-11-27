---
title: "Klass Line"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Line-klass. Inkapslar objektet som representerar linjeformatet"
type: docs
url: /sv/net/aspose.cells.drawing/line/
---
## Line class

Inkapslar objektet som representerar linjeformatet.

```csharp
public class Line
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Anger längden på pilspetsen för början av en linje. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Anger bredden på pilspetsen för början av en linje. |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Anger en pilspets för början av en linje. |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Anger slutkapparna. |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Representerar färgen på linjen. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Anger den sammansatta linjetypen |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Anger strecklinjetypen |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Anger längden på pilspetsen för slutet av en linje. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Anger bredden på pilspetsen för slutet av en linje. |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Anger en pilspets för slutet av en linje. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Hämtar eller anger formattyp. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Representerar gradientfyllning. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indikerar om den här linjestilen är automatiskt tilldelad. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indikerar om linjens färg tilldelas automatiskt. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Anger om linjen är synlig. |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Specificerar sammankopplingsändarna. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Anger linjens stil. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Hämtar och anger temafärgen. |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Returnerar eller anger transparensgraden för linjen som ett värde från 0.0 (opak) till 1.0 (klar). |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Hämtar eller anger [`WeightType`](../weighttype/) för linjen. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Hämtar eller anger linjens tjocklek i enheter av punkter. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Hämtar eller anger linjens vikt i pixlar. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


