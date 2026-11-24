---
title: "Trendline.Backward"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Trendline-Eigenschaft. Gibt die Anzahl der Perioden oder Einheiten in einem Streudiagramm zurück oder legt sie fest, um die die Trendlinie nach hinten erweitert wird. Die Anzahl der Perioden muss größer oder gleich null sein. Wenn der Diagrammtyp Säule ist, muss die Anzahl der Perioden zwischen 0 und 0,5 liegen."
type: docs
url: /de/net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

Liefert oder setzt die Anzahl der Perioden (oder Einheiten in einem Streudiagramm), um die die Trendlinie rückwärts verlängert wird. Die Anzahl der Perioden muss größer oder gleich null sein. Wenn der Diagrammtyp Säule ist, muss die Anzahl der Perioden zwischen 0 und 0,5 liegen.

```csharp
public double Backward { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Trendlinie hinzufügen und sie über den Index abrufen.
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Setze die Backward-Eigenschaft, um die Trendlinie um 0,5 Einheiten nach hinten zu erweitern.
            trendline.Backward = 0.5;
            
            workbook.Save("TrendlineBackwardDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


