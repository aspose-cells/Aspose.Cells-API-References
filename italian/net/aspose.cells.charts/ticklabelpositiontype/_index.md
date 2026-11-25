---
title: "Enum TickLabelPositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.TickLabelPositionType enum. Rappresenta il tipo di posizione delle etichette dei segni di graduazione sull'asse specificato"
type: docs
url: /it/net/aspose.cells.charts/ticklabelpositiontype/
---
## TickLabelPositionType enumeration

Rappresenta il tipo di posizione delle etichette dei segni sull'asse specificato.

```csharp
public enum TickLabelPositionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| High | `0` | Il tipo di posizione è alto. |
| Low | `1` | Il tipo di posizione è basso. |
| NextToAxis | `2` | Il tipo di posizione è accanto all'asse. |
| None | `3` | Il tipo di posizione è nessuno. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelPositionTypeDemo
    {
        public static void TickLabelPositionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Accedi all'asse delle categorie
            Axis categoryAxis = chart.CategoryAxis;
            
            // Imposta la posizione dell'etichetta di graduazione su Alto
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // Salva la cartella di lavoro
            workbook.Save("TickLabelPositionTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


