---
title: "ChartPoint.Marker"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint‑egenskap. Hämtar markören"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/marker/
---
## ChartPoint.Marker property

Hämtar ` marker`.

```csharp
public Marker Marker { get; }
```

### Exempel

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
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(150);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(33);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Scatter, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // Anpassa markören för den första punkten
            int pointIndex = 0;
            chart.NSeries[0].Points[pointIndex].Marker.Border.Color = Color.Yellow;
            chart.NSeries[0].Points[pointIndex].Marker.Area.ForegroundColor = Color.Green;
            chart.NSeries[0].Points[pointIndex].Marker.MarkerStyle = Aspose.Cells.Charts.ChartMarkerType.Circle;
            chart.NSeries[0].Points[pointIndex].Marker.MarkerSize = 16;
            
            // Spara arbetsboken
            workbook.Save("ChartPointMarkerDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Marker](../../marker/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


