---
title: "Class DropBars"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.DropBars class. Rappresenta le barre su e giù in un grafico"
type: docs
url: /it/net/aspose.cells.charts/dropbars/
---
## DropBars class

Rappresenta le barre su e giù in un grafico.

```csharp
public class DropBars
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Area](../../aspose.cells.charts/dropbars/area/) { get; } | Ottiene il [`Area`](./area/). |
| [Border](../../aspose.cells.charts/dropbars/border/) { get; } | Ottiene il bordo [`Line`](../../aspose.cells.drawing/line/). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsDemo
    {
        public static void DropBarsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B3"
            chart.NSeries.Add("A1:B3", true);

            // Abilita le barre su e giù
            chart.NSeries[0].HasUpDownBars = true;

            // Accedi all'oggetto DropBars
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // Personalizza l'aspetto delle barre su
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // Personalizza l'aspetto delle barre giù
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // Salva la cartella di lavoro
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


