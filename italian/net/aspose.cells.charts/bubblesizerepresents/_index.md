---
title: "Enum BubbleSizeRepresents"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.BubbleSizeRepresents enum. Rappresenta ciò che la dimensione della bolla indica in un grafico a bolle."
type: docs
url: /it/net/aspose.cells.charts/bubblesizerepresents/
---
## BubbleSizeRepresents enumeration

Rappresenta ciò che la dimensione della bolla indica in un grafico a bolle.

```csharp
public enum BubbleSizeRepresents
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| SizeIsArea | `0` | Rappresenta il valore di [`BubbleSizes`](../series/bubblesizes/), che è l'area della bolla. |
| SizeIsWidth | `1` | Rappresenta il valore di [`BubbleSizes`](../series/bubblesizes/), che è la larghezza della bolla. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class BubbleSizeRepresentsDemo
    {
        public static void BubbleSizeRepresentsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico a bolle
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // Aggiungi un grafico a bolle al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie al grafico a bolle
            int seriesIndex = chart.NSeries.Add("A1:C3", true);
            Series series = chart.NSeries[seriesIndex];

            // Imposta i valori X, i valori Y e le dimensioni delle bolle
            series.XValues = "A1:A3";
            series.Values = "B1:B3";
            series.BubbleSizes = "C1:C3";

            // Imposta la rappresentazione della dimensione della bolla
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Salva la cartella di lavoro
            workbook.Save("BubbleSizeRepresentsExample.xlsx");
            workbook.Save("BubbleSizeRepresentsExample.pdf");

            // Imposta la rappresentazione della dimensione della bolla
            series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            // Salva la cartella di lavoro
            workbook.Save("BubbleSizeRepresentsExample2.xlsx");
            workbook.Save("BubbleSizeRepresentsExample2.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


