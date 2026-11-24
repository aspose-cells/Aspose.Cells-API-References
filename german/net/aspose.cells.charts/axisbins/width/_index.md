---
title: "AxisBins.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AxisBins-Eigenschaft. Liest oder setzt die Breite des Achsen-Bins"
type: docs
url: /de/net/aspose.cells.charts/axisbins/width/
---
## AxisBins.Width property

Liest oder legt die Breite des Achsenbehälters fest.

```csharp
public double Width { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);

            // Histogramm-Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 7, 1, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.CategoryData = "B1:D1";

            // Bin-Breite festlegen
            chart.CategoryAxis.Bins.Width = 12;

            // Speichere und demonstriere das Ergebnis
            workbook.Save("AxisBinsPropertyWidthDemo_out.xlsx");

            Console.WriteLine("Example executed successfully with bin width set to 12.");
        }
    }
}
```

### Siehe auch

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


