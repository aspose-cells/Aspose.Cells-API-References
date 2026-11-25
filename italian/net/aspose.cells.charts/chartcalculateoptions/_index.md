---
title: "Classe ChartCalculateOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.ChartCalculateOptions. Rappresenta le opzioni per il calcolo di un grafico"
type: docs
url: /it/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

Rappresenta le opzioni per il calcolo di un grafico.

```csharp
public class ChartCalculateOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | Crea le opzioni per il calcolo del grafico. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | Indica se aggiornare tutti i punti dati durante l'esecuzione del calcolo del grafico. Predefinito: False. Quando si desidera ottenere il valore di ciascun punto dati nel grafico in modo specifico, impostarlo su true. Se questo parametro è impostato su True, i nuovi punti dati possono essere generati quando il grafico viene calcolato. Questo potrebbe aumentare le dimensioni del file Excel. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
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

            // Crea un'istanza di ChartCalculateOptions
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // Calcola il grafico con le opzioni specificate
            chart.Calculate(options);

            // Salva la cartella di lavoro
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


