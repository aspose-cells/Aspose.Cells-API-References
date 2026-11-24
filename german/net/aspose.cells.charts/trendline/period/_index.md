---
title: "Trendline.Period"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Trendline-Eigenschaft. Gibt den Zeitraum für die MovingAverage-Trendlinie zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.charts/trendline/period/
---
## Trendline.Period property

Gibt die Periode für die gleitende Mittelwert-Trendlinie zurück oder setzt sie.

```csharp
public int Period { get; set; }
```

### Hinweise

Dieser Wert sollte zwischen 2 und 255 liegen. Und er muss kleiner sein als die Anzahl der Diagrammpunkte in der Serie.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyPeriodDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Serie hinzufügen
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Eine MovingAverage-Trendlinie hinzufügen.
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Period = 3; // Set period for moving average
            trendline.Name = "3-Period Moving Average";

            // Speichere die Arbeitsmappe
            workbook.Save("TrendlinePeriodDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


