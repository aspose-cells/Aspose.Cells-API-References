---
title: "AxisBins.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AxisBins. Ottiene o imposta la larghezza del contenitore dell'asse"
type: docs
url: /it/net/aspose.cells.charts/axisbins/width/
---
## AxisBins.Width property

Ottiene o imposta la larghezza del cestino dell'asse.

```csharp
public double Width { get; set; }
```

### Esempi

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

            // Dati di esempio
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);

            // Crea grafico a istogramma
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 7, 1, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.CategoryData = "B1:D1";

            // Imposta la larghezza del contenitore
            chart.CategoryAxis.Bins.Width = 12;

            // Salva e dimostra il risultato
            workbook.Save("AxisBinsPropertyWidthDemo_out.xlsx");

            Console.WriteLine("Example executed successfully with bin width set to 12.");
        }
    }
}
```

### Vedi anche

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


