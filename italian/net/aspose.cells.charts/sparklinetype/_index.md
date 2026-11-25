---
title: "Enum SparklineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.SparklineType enum. Rappresenta i tipi di sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinetype/
---
## SparklineType enumeration

Rappresenta i tipi di sparkline.

```csharp
public enum SparklineType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Line | `0` | Sparkline a linea. |
| Column | `1` | Sparkline di colonna. |
| Stacked | `2` | Rappresenta una sparkline Vincita/Perdita. |
| WinLoss | `2` | Rappresenta una sparkline Vincita/Perdita. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineTypeDemo
    {
        public static void SparklineTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Definisci il CellArea per lo sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi un gruppo di sparkline al foglio di lavoro
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Aggiungi sparkline al gruppo
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Personalizza il gruppo di sparkline
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Imposta i punti alti per essere colorati di verde e i punti bassi per essere colorati di rosso
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Imposta lo spessore della linea
            group.LineWeight = 1.0;

            // Salva la cartella di lavoro
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


