---
title: "Klasse SlicerCacheItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Slicers.SlicerCacheItem Klasse. Stellt ein Slicer-Datenquellen-Element dar."
type: docs
url: /de/net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

Stellt das Slicer‑Datenquellen‑Element dar

```csharp
public class SlicerCacheItem
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | Gibt an, ob das `SlicerCacheItem` ausgewählt ist oder nicht. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Gibt den Beschriftungstext für das Slicer-Element zurück. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerCacheItemDemo
    {
        public static void Run()
        {
            // Lade die Arbeitsmappe mit Slicer
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // Hole den ersten Slicer in der Arbeitsmappe
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // Durchlaufe die Slicer-Cache-Elemente
            Console.WriteLine("Slicer Cache Items:");
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
                Console.WriteLine($"Item {i}: Selected={slicerCacheItem.Selected}, Value={slicerCacheItem.Value}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


