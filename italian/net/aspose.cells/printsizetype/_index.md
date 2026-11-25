---
title: "Enum PrintSizeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.PrintSizeType. Rappresenta la dimensione del grafico stampato"
type: docs
url: /it/net/aspose.cells/printsizetype/
---
## PrintSizeType enumeration

Rappresenta la dimensione del grafico stampato.

```csharp
public enum PrintSizeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Full | `0` | Usa l'intera pagina. |
| Fit | `1` | Scala per adattare alla pagina. |
| Custom | `2` | Personalizzato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PrintSizeTypeDemo
    {
        public static void PrintSizeTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo di dati per il grafico
            chart.SetChartDataRange("A1:B4", true);

            // Imposta il titolo del grafico
            chart.Title.Text = "Sample Chart";

            // Imposta la dimensione di stampa del grafico
            chart.PrintSize = PrintSizeType.Fit;

            // Salva la cartella di lavoro
            workbook.Save("PrintSizeTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


