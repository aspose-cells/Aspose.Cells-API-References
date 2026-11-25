---
title: "Enum ErrorBarDisplayType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.ErrorBarDisplayType enum. Rappresenta il tipo di visualizzazione della barra di errore"
type: docs
url: /it/net/aspose.cells.charts/errorbardisplaytype/
---
## ErrorBarDisplayType enumeration

Rappresenta il tipo di visualizzazione della barra di errore.

```csharp
public enum ErrorBarDisplayType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Both | `0` | Entrambi |
| Minus | `1` | Meno |
| None | `2` | Nessuno |
| Plus | `3` | Più |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDisplayTypeDemo
    {
        public static void ErrorBarDisplayTypeExample()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue(2);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(6);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(7);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Aggiungi un grafico a colonne al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Configura le barre di errore per ogni serie nel grafico
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Salva la cartella di lavoro
            workbook.Save("ErrorBarDisplayTypeExample.xlsx");
            workbook.Save("ErrorBarDisplayTypeExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


