---
title: "AxisBins.Underflow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AxisBins. Ottiene o imposta l'underflow dei contenitori dell'asse"
type: docs
url: /it/net/aspose.cells.charts/axisbins/underflow/
---
## AxisBins.Underflow property

Ottiene o imposta l'underflow dei cestini dell'asse

```csharp
public double Underflow { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["C1"].PutValue(20);
            worksheet.Cells["D1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["C2"].PutValue(32);
            worksheet.Cells["D2"].PutValue(31);
            worksheet.Cells["B3"].PutValue(185);
            worksheet.Cells["C3"].PutValue(202);
            worksheet.Cells["D3"].PutValue(224);

            // Aggiungi grafico a istogramma
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 7, 1, 25, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:D2", false);
            chart.NSeries.Add("B3:D3", false);
            chart.NSeries.CategoryData = "B1:D1";

            // Configura le proprietà dei contenitori
            var bins = chart.CategoryAxis.Bins;
            bins.Width = 12;
            bins.Count = 3;
            bins.Overflow = 10;
            bins.Underflow = 0.5; // Demonstrate Underflow property

            // Salva la cartella di lavoro
            workbook.Save("AxisBinsPropertyUnderflowDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


