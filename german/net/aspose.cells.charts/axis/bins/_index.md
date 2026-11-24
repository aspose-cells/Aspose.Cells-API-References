---
title: "Axis.Bins"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Achsen-Eigenschaft. Stellt Klassen auf einer Diagramm‑Histogramm/Pareto-Achse dar"
type: docs
url: /de/net/aspose.cells.charts/axis/bins/
---
## Axis.Bins property

Stellt Bins auf einer Diagramm(Histogramm/Pareto)-Achse dar

```csharp
public AxisBins Bins { get; }
```

### Hinweise

Nur für Histogramm- oder Pareto-Diagramm.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBinsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Histogramm-Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Bins konfigurieren
            AxisBins bins = chart.ValueAxis.Bins;
            bins.IsAutomatic = false;
            bins.Width = 15;
            bins.Overflow = 55;
            bins.Underflow = 5;

            workbook.Save("AxisBinsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AxisBins](../../axisbins/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


