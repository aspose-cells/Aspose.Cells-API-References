---
title: "SparklineGroupCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroupCollection-Eigenschaft. Gibt das SparklineGroup-Element am angegebenen Index zurück."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

Gibt das [`SparklineGroup`](../../sparklinegroup/) Element am angegebenen Index zurück.

```csharp
public SparklineGroup this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

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
            
            // Fügen Sie Beispieldaten hinzu
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            ws.Cells["A3"].PutValue(7);
            ws.Cells["A4"].PutValue(2);
            ws.Cells["A5"].PutValue(9);

            // Definieren Sie den Datenbereich und den Ort für Sparklines
            string dataRange = "'" + ws.Name + "'!A1:A5";
            CellArea location = new CellArea();
            location.StartRow = 0;
            location.EndRow = 0;
            location.StartColumn = 1;
            location.EndColumn = 1;

            // Sparkline-Gruppe hinzufügen
            int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
            
            // Greifen Sie auf die Sparkline-Gruppe über die Item-Eigenschaft zu
            SparklineGroup group = ws.SparklineGroups[index];
            
            // Passen Sie die Sparkline an
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Speichere die Arbeitsmappe
            wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


