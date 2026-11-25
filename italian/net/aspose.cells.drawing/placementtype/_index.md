---
title: "Enum PlacementType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.PlacementType enum. Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti."
type: docs
url: /it/net/aspose.cells.drawing/placementtype/
---
## PlacementType enumeration

Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti.

```csharp
public enum PlacementType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| FreeFloating | `0` | Non spostare né ridimensionare con le celle. |
| Move | `1` | Sposta ma non ridimensionare con le celle. |
| MoveAndSize | `2` | Sposta e ridimensiona con le celle. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class PlacementTypeDemo
    {
        public static void PlacementTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Imposta il tipo di posizionamento del grafico
            chart.Placement = PlacementType.MoveAndSize;

            // Restituisci il tipo di posizionamento
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // Salva la cartella di lavoro
            workbook.Save("PlacementTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


