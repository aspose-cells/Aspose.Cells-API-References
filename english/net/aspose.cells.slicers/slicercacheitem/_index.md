---
title: Class SlicerCacheItem
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Slicers.SlicerCacheItem class. Represent slicer data source item
type: docs
url: /net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

Represent slicer data source item

```csharp
public class SlicerCacheItem
```

## Properties

| Name | Description |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | Specifies whether the SlicerItem is selected or not. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Returns the label text for the slicer item. |

### Examples

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
            // Load the workbook with slicer
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // Get the first slicer in the workbook
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // Iterate through slicer cache items
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

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


