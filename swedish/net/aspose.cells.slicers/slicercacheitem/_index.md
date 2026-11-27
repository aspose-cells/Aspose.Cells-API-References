---
title: "Klass SlicerCacheItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Slicers.SlicerCacheItem-klass. Representerar slicer-datakällans objekt"
type: docs
url: /sv/net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

Representerar slicer-datakällapost.

```csharp
public class SlicerCacheItem
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | Anger om `SlicerCacheItem` är markerad eller inte. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Returnerar etiketttexten för skärmningsobjektet. |

### Exempel

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
            // Läs in arbetsboken med skärmningskontrollen.
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // Hämta den första skärmningskontrollen i arbetsboken.
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // Iterera genom skärmningscache‑objekten.
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

### Se även

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


