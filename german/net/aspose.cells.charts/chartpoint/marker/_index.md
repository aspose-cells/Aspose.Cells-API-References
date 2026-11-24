---
title: "ChartPoint.Marker"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt den Marker zurück."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/marker/
---
## ChartPoint.Marker property

Gibt den ` marker` zurück.

```csharp
public Marker Marker { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(150);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(33);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Scatter, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // Passe den Marker für den ersten Punkt an.
            int pointIndex = 0;
            chart.NSeries[0].Points[pointIndex].Marker.Border.Color = Color.Yellow;
            chart.NSeries[0].Points[pointIndex].Marker.Area.ForegroundColor = Color.Green;
            chart.NSeries[0].Points[pointIndex].Marker.MarkerStyle = Aspose.Cells.Charts.ChartMarkerType.Circle;
            chart.NSeries[0].Points[pointIndex].Marker.MarkerSize = 16;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointMarkerDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Marker](../../marker/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


