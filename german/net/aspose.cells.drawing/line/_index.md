---
title: "Klasse Line"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Line-Klasse. Kapselt das Objekt, das das Linienformat darstellt."
type: docs
url: /de/net/aspose.cells.drawing/line/
---
## Line class

Kapselt das Objekt, das das Linienformat darstellt.

```csharp
public class Line
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Gibt die Länge der Pfeilspitze für den Anfang einer Linie an. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Gibt die Breite der Pfeilspitze für den Anfang einer Linie an. |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Gibt eine Pfeilspitze für den Anfang einer Linie an. |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Gibt die Endkappen an. |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Stellt die Farbe der Linie dar. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Gibt den zusammengesetzten Linientyp an |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Gibt den Strichlinientyp an |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Gibt die Länge der Pfeilspitze für das Ende einer Linie an. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Gibt die Breite der Pfeilspitze für das Ende einer Linie an. |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Gibt eine Pfeilspitze für das Ende einer Linie an. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Ruft den Formattyp ab oder legt ihn fest. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Stellt einen Farbverlauf dar. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Gibt an, ob dieser Linienstil automatisch zugewiesen wird. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Gibt an, ob die Farbe der Linie automatisch zugewiesen wird. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Stellt dar, ob die Linie sichtbar ist. |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Gibt die Verbindungsenden an. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Stellt den Stil der Linie dar. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Liest und setzt die Themenfarbe. |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Gibt den Transparenzgrad der Linie zurück oder legt ihn fest, als Wert von 0.0 (undurchsichtig) bis 1.0 (transparent). |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Ermittelt oder legt den [`WeightType`](../weighttype/) der Linie fest. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Liest oder setzt die Stärke der Linie in Punkten. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Ermittelt oder legt das Gewicht der Linie in Pixeln fest. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


