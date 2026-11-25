---
title: "Series.BubbleSizes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene o imposta i valori delle dimensioni delle bolle della serie del grafico"
type: docs
url: /it/net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

Ottiene o imposta i valori di dimensione delle bolle della serie del grafico.

```csharp
public string BubbleSizes { get; set; }
```

### Osservazioni

Solo per Bubble o Bubble3D.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleSizesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico a bolle
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["C1"].PutValue("Bubble Sizes");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
                worksheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Aggiungi un grafico a bolle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta i dati della serie usando la proprietà BubbleSizes
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";
            chart.NSeries[0].BubbleSizes = "C2:C5";

            // Salva la cartella di lavoro
            workbook.Save("BubbleChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


