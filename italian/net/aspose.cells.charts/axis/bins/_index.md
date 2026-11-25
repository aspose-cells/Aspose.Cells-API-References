---
title: "Axis.Bins"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta i contenitori su un asse del grafico Istogramma/Pareto"
type: docs
url: /it/net/aspose.cells.charts/axis/bins/
---
## Axis.Bins property

Rappresenta i contenitori su un asse di grafico (Istogramma/Pareto)

```csharp
public AxisBins Bins { get; }
```

### Osservazioni

Solo per grafico Istogramma o Pareto.

### Esempi

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

            // Dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Crea grafico a istogramma
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Configura i contenitori
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

### Vedi anche

* class [AxisBins](../../axisbins/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


