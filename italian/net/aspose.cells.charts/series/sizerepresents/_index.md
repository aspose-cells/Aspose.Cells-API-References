---
title: "Series.SizeRepresents"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene o imposta cosa rappresenta la dimensione della bolla in un grafico a bolle"
type: docs
url: /it/net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

Ottiene o imposta cosa rappresenta la dimensione della bolla in un grafico a bolle.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### Osservazioni

BubbleSizeRepresents.SizeIsArea indica che il valore [`BubbleSizes`](../bubblesizes/) è l'area della bolla. BubbleSizeRepresents.SizeIsWidth indica che il valore [`BubbleSizes`](../bubblesizes/) è la larghezza della bolla.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySizeRepresentsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico a bolle
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["C1"].PutValue("Size");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
                sheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Aggiungi un grafico a bolle
            int chartIndex = sheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta i dati della serie
            SeriesCollection series = chart.NSeries;
            series.Add("B2:B5", true);
            series.CategoryData = "A2:A5";
            series[0].BubbleSizes = "C2:C5";

            // Imposta la proprietà SizeRepresents
            series[0].SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertySizeRepresentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


