---
title: "SparklineCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineCollection-egenskap. Hämtar Sparkline-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.charts/sparklinecollection/item/
---
## SparklineCollection indexer

Hämtar [`Sparkline`](../../sparkline/) elementet på det angivna indexet.

```csharp
public Sparkline this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);

            // Skapa sparkline-grupp
            SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;
            int idx = sparklineGroups.Add(SparklineType.Line, "A1:D1", false, CellArea.CreateCellArea(0, 4, 0, 4));
            SparklineGroup group = sparklineGroups[idx];

            // Åtkomst till sparklines via Item-egenskapen
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline Data Range: " + sparkline.DataRange);
            Console.WriteLine("Sparkline Type: " + group.Type);

            // Modifiera sparkline-data
            worksheet.Cells["A1"].PutValue(8);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


