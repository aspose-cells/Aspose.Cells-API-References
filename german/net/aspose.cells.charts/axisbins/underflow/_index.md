---
title: "AxisBins.Underflow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AxisBins-Eigenschaft. Liest oder setzt den Unterlauf der Achsen-Bins"
type: docs
url: /de/net/aspose.cells.charts/axisbins/underflow/
---
## AxisBins.Underflow property

Liest oder legt den Unterlauf der Achsenbehälter fest

```csharp
public double Underflow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyUnderflowDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);
            worksheet.Cells["B3"].PutValue(185);
            worksheet.Cells["C3"].PutValue(202);
            worksheet.Cells["D3"].PutValue(224);

            // Histogramm-Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 7, 1, 25, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.Add("B3:D3", false);
            chart.NSeries.CategoryData = "B1:D1";

            // Bins-Eigenschaften konfigurieren
            var bins = chart.CategoryAxis.Bins;
            bins.Width = 12;
            bins.Count = 3;
            bins.Overflow = 10;
            bins.Underflow = 0.5; // Demonstrate Underflow property

            // Speichere die Arbeitsmappe
            workbook.Save("AxisBinsPropertyUnderflowDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


