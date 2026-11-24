---
title: "Trendline.Intercept"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Trendline‑Eigenschaft. Gibt den Punkt zurück oder legt ihn fest, an dem die Trendlinie die Werteachse schneidet"
type: docs
url: /de/net/aspose.cells.charts/trendline/intercept/
---
## Trendline.Intercept property

Gibt den Punkt zurück, an dem die Trendlinie die Werteachse schneidet, oder setzt ihn.

```csharp
public double Intercept { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyInterceptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Trendlinie hinzufügen und Schnittpunkt festlegen
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Intercept = 1.0; // Setting the Y-intercept value
            trendline.DisplayEquation = true;

            workbook.Save("TrendlineInterceptDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


