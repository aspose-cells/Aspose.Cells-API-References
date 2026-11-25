---
title: "SparklineCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "proprietà SparklineCollection. Ottiene l'elemento Sparkline all'indice specificato"
type: docs
url: /it/net/aspose.cells.charts/sparklinecollection/item/
---
## SparklineCollection indexer

Ottiene l'elemento [`Sparkline`](../../sparkline/) all'indice specificato.

```csharp
public Sparkline this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);

            // Crea gruppo sparkline
            SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;
            int idx = sparklineGroups.Add(SparklineType.Line, "A1:D1", false, CellArea.CreateCellArea(0, 4, 0, 4));
            SparklineGroup group = sparklineGroups[idx];

            // Accedi agli sparkline usando la proprietà Item
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline Data Range: " + sparkline.DataRange);
            Console.WriteLine("Sparkline Type: " + group.Type);

            // Modifica i dati dello sparkline
            worksheet.Cells["A1"].PutValue(8);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


