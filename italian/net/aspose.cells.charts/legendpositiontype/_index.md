---
title: "Enum LegendPositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.LegendPositionType enum. Elenca i tipi di posizione della legenda"
type: docs
url: /it/net/aspose.cells.charts/legendpositiontype/
---
## LegendPositionType enumeration

Enumera i tipi di posizione della legenda.

```csharp
public enum LegendPositionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Bottom | `0` | Visualizza la legenda nella parte inferiore dell'area di tracciamento del grafico. |
| Corner | `1` | Visualizza la legenda nell'angolo dell'area di tracciamento del grafico. |
| Left | `4` | Visualizza la legenda a sinistra dell'area di tracciamento del grafico. |
| NotDocked | `7` | Indica che la legenda non è ancorata. |
| Right | `3` | Visualizza la legenda a destra dell'area di tracciamento del grafico. |
| Top | `2` | Visualizza la legenda nella parte superiore dell'area di tracciamento del grafico. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPositionTypeDemo
    {
        public static void LegendPositionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Aggiungi un grafico a colonne al foglio di lavoro
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accedi alla legenda del grafico
            Legend legend = chart.Legend;

            // Imposta la posizione della legenda a sinistra del grafico
            legend.Position = LegendPositionType.Left;

            // Imposta proprietà aggiuntive per la legenda
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // Salva la cartella di lavoro
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


