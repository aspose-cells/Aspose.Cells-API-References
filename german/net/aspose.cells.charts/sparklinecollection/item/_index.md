---
title: "SparklineCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineCollection-Eigenschaft. Gibt das Sparkline-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.charts/sparklinecollection/item/
---
## SparklineCollection indexer

Gibt das [`Sparkline`](../../sparkline/) Element am angegebenen Index zurück.

```csharp
public Sparkline this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);

            // Sparkline-Gruppe erstellen
            SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;
            int idx = sparklineGroups.Add(SparklineType.Line, "A1:D1", false, CellArea.CreateCellArea(0, 4, 0, 4));
            SparklineGroup group = sparklineGroups[idx];

            // Greife auf Sparklines über die Item-Eigenschaft zu
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline Data Range: " + sparkline.DataRange);
            Console.WriteLine("Sparkline Type: " + group.Type);

            // Sparkline-Daten ändern
            worksheet.Cells["A1"].PutValue(8);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


