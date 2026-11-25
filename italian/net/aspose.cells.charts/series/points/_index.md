---
title: "Series.Points"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene la collezione di punti in una serie in un grafico"
type: docs
url: /it/net/aspose.cells.charts/series/points/
---
## Series.Points property

Ottiene la raccolta di punti in una serie in un grafico.

```csharp
public ChartPointCollection Points { get; }
```

### Osservazioni

Quando il grafico è Pie of Pie o Bar of Pie, l'ultimo punto è un altro punto nel primo grafico a torta.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPointsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alla prima serie e ai suoi punti
            Series series = chart.NSeries[0];
            foreach (ChartPoint point in series.Points)
            {
                // Aggiungi etichette dati a ogni punto
                point.DataLabels.ShowValue = true;
                point.DataLabels.ShowCellRange = true;
            }

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


