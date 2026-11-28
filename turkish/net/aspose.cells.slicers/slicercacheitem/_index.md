---
title: "Sınıf SlicerCacheItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Slicers.SlicerCacheItem sınıfı. Slicer veri kaynağı öğesini temsil eder"
type: docs
url: /tr/net/aspose.cells.slicers/slicercacheitem/
---
## SlicerCacheItem class

Dilimleyici veri kaynağı öğesini temsil eder

```csharp
public class SlicerCacheItem
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Selected](../../aspose.cells.slicers/slicercacheitem/selected/) { get; set; } | `SlicerCacheItem`'in seçili olup olmadığını belirtir. |
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Slicer öğesi için etiket metnini döndürür. |

### Örnekler

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
            // Slicer içeren çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsx");
            workbook.Worksheets.RefreshAll();

            // Çalışma kitabındaki ilk slicer'ı al
            var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

            // Slicer önbellek öğeleri arasında yinele
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


