---
title: "Series.ShowNegativeBubbles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà della serie. True se le bolle negative sono mostrate per il gruppo di grafico. Valido solo per i grafici a bolle"
type: docs
url: /it/net/aspose.cells.charts/series/shownegativebubbles/
---
## Series.ShowNegativeBubbles property

Vero se le bolle negative sono visualizzate per il gruppo del grafico. Valido solo per i grafici a bolle.

```csharp
public bool ShowNegativeBubbles { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShowNegativeBubblesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico a bolle
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(-3);
            worksheet.Cells["B4"].PutValue(4);
            
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(6);
            worksheet.Cells["C4"].PutValue(7);

            // Aggiungi un grafico a bolle
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            seriesCollection.CategoryData = "A2:A4";
            seriesCollection[0].BubbleSizes = "C2:C4";

            // Accedi alla prima serie e imposta la proprietà ShowNegativeBubbles
            Series series = chart.NSeries[0];
            series.ShowNegativeBubbles = true;

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


