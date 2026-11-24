---
title: "Klasse Marker"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.Marker Klasse. Stellt den Marker in einem Liniendiagramm, Streudiagramm oder Radar-Diagramm dar"
type: docs
url: /de/net/aspose.cells.charts/marker/
---
## Marker class

Stellt den Marker in einem Liniendiagramm, Streudiagramm oder Radar­diagramm dar.

```csharp
public class Marker
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | Liest das [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | Stellt die Hintergrundfarbe des Markers in einem Liniendiagramm, Streudiagramm oder Radar-Diagramm dar. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | Liest oder setzt den Typ der Hintergrundfarbeneinstellung des Markers. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | Liest das [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | Stellt die Vordergrundfarbe des Markers in einem Liniendiagramm, Streudiagramm oder Radar-Diagramm dar. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | Liest oder setzt den Typ der Vordergrundfarbeneinstellung des Markers. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | Stellt die Markergöße in Punkt als Einheit dar. Gilt für Liniendiagramme, Streudiagramme oder Radar-Diagramme. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | Stellt die Markergöße in Pixeln dar. Gilt für Liniendiagramme, Streudiagramme oder Radar-Diagramme. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | Stellt den Markerstil dar. Gilt für ein Liniendiagramm, ein Streudiagramm oder ein Radar-Diagramm. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MarkerDemo
    {
        public static void MarkerExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Holen Sie die Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Füge NSeries (Diagrammdatenquelle) zum Diagramm hinzu, das vom Feld "A1" bis "B3" reicht.
            chart.NSeries.Add("A1:B3", true);

            // Zugriff auf die erste Serie
            Series series = chart.NSeries[0];

            // Marker-Eigenschaften festlegen
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // Speichere die Arbeitsmappe
            workbook.Save("MarkerExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


