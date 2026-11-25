---
title: "SparklineGroupCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroupCollection. Ottiene l'elemento SparklineGroup all'indice specificato."
type: docs
url: /it/net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

Ottiene l'elemento [`SparklineGroup`](../../sparklinegroup/) all'indice specificato.

```csharp
public SparklineGroup this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Aggiungi dati di esempio
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            ws.Cells["A3"].PutValue(7);
            ws.Cells["A4"].PutValue(2);
            ws.Cells["A5"].PutValue(9);

            // Definisci l'intervallo di dati e la posizione per gli sparklines.
            string dataRange = "'" + ws.Name + "'!A1:A5";
            CellArea location = new CellArea();
            location.StartRow = 0;
            location.EndRow = 0;
            location.StartColumn = 1;
            location.EndColumn = 1;

            // Aggiungi gruppo di sparkline
            int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
            
            // Accedi al gruppo di sparkline usando la proprietà Item
            SparklineGroup group = ws.SparklineGroups[index];
            
            // Personalizza lo sparkline
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Salva la cartella di lavoro
            wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


