---
title: "TrendlineCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TrendlineCollection. Ottiene un oggetto Trendline per il suo indice"
type: docs
url: /it/net/aspose.cells.charts/trendlinecollection/item/
---
## TrendlineCollection indexer

Ottiene un oggetto [`Trendline`](../../trendline/) per il suo indice.

```csharp
public Trendline this[int index] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(1);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(3);
            sheet.Cells["B1"].PutValue(4);
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(6);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Values = "B1:B3";

            // Aggiungi una trendline
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];

            // Dimostra l'uso della proprietà Item
            Trendline firstTrendline = chart.NSeries[0].TrendLines[0];
            Console.WriteLine("Trendline Type: " + firstTrendline.Type);
        }
    }
}
```

### Vedi anche

* class [Trendline](../../trendline/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


