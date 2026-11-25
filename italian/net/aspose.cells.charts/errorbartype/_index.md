---
title: "Enum ErrorBarType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.ErrorBarType enum. Rappresenta il tipo di quantità della barra di errore"
type: docs
url: /it/net/aspose.cells.charts/errorbartype/
---
## ErrorBarType enumeration

Rappresenta il tipo di quantità della barra di errore.

```csharp
public enum ErrorBarType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Custom | `0` | Tipo di valore InnerCustom. |
| FixedValue | `1` | Tipo di valore fisso. |
| Percent | `2` | Tipo percentuale |
| StDev | `3` | Tipo deviazione standard. |
| StError | `4` | Tipo errore standard. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarTypeDemo
    {
        public static void ErrorBarTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Aggiungi alcuni dati di esempio
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);

            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Imposta le proprietà della barra di errore per ogni serie nel grafico
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Salva la cartella di lavoro
            workbook.Save("ErrorBarTypeExample.xlsx");
            workbook.Save("ErrorBarTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


