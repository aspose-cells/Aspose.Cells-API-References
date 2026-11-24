---
title: "Marker.BackgroundColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Marker-Eigenschaft. Gibt die Hintergrundfarbe des Markers in einem Liniendiagramm, Streudiagramm oder Radar-Diagramm an"
type: docs
url: /de/net/aspose.cells.charts/marker/backgroundcolor/
---
## Marker.BackgroundColor property

Stellt die Hintergrundfarbe des Markers in einem Liniendiagramm, Streudiagramm oder Radar-Diagramm dar.

```csharp
public Color BackgroundColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Marker‑Aussehen anpassen
            foreach (Series series in chart.NSeries)
            {
                series.Marker.MarkerStyle = ChartMarkerType.Circle;
                series.Marker.MarkerSize = 12;
                series.Marker.Border.Color = System.Drawing.Color.Blue;
                series.Marker.BackgroundColor = System.Drawing.Color.LightGreen; // Demonstrating BackgroundColor property
            }

            workbook.Save("MarkerBackgroundColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


