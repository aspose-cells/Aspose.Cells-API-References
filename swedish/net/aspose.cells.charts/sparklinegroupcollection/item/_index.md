---
title: "SparklineGroupCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroupCollection‑egenskap. Hämtar SparklineGroup‑elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

Hämtar [`SparklineGroup`](../../sparklinegroup/) elementet på det angivna indexet.

```csharp
public SparklineGroup this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

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
            
            // Lägg till exempeldata
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            ws.Cells["A3"].PutValue(7);
            ws.Cells["A4"].PutValue(2);
            ws.Cells["A5"].PutValue(9);

            // Definiera dataområde och plats för sparklines
            string dataRange = "'" + ws.Name + "'!A1:A5";
            CellArea location = new CellArea();
            location.StartRow = 0;
            location.EndRow = 0;
            location.StartColumn = 1;
            location.EndColumn = 1;

            // Lägg till sparkline-grupp
            int index = ws.SparklineGroups.Add(SparklineType.Line, dataRange, false, location);
            
            // Åtkomst till sparkline-gruppen med Item‑egenskapen
            SparklineGroup group = ws.SparklineGroups[index];
            
            // Anpassa sparkline
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Spara arbetsboken
            wb.Save("SparklineGroupCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


