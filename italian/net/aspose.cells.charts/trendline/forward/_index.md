---
title: "Trendline.Forward"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Trendline. Restituisce o imposta il numero di periodi o unità su un grafico a dispersione a cui la trendline si estende in avanti. Il numero di periodi deve essere maggiore o uguale a zero"
type: docs
url: /it/net/aspose.cells.charts/trendline/forward/
---
## Trendline.Forward property

Restituisce o imposta il numero di periodi (o unità in un grafico a dispersione) a cui la linea di tendenza si estende in avanti. Il numero di periodi deve essere maggiore o uguale a zero.

```csharp
public double Forward { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyForwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Aggiungi linea di tendenza
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Dimostrare la proprietà Forward
            trendline.Forward = 2.5; // Extend trendline forward by 2.5 units
            
            workbook.Save("TrendlineForwardDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


