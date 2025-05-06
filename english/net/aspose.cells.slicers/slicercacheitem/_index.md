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
| [Value](../../aspose.cells.slicers/slicercacheitem/value/) { get; } | Returns the label text for the slicer item. Read-only. |

### Examples

```csharp
// Called: foreach (SlicerCacheItem cacheItem in slicer.SlicerCache.SlicerCacheItems)
[Test]
        public void Type_SlicerCacheItem()
        {
            var wb = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET54826.xlsx&quot;);
            var ws = wb.Worksheets[0];
            ws.RefreshPivotTables();

            var targetCell = ws.Cells[&quot;E1&quot;];
            // print: (All)
            Console.WriteLine(targetCell.Value);

            var slicer = ws.Slicers[0];
            // select alex
            foreach (SlicerCacheItem cacheItem in slicer.SlicerCache.SlicerCacheItems)
            {
                cacheItem.Selected = cacheItem.Value == &quot;Alex&quot;;
            }
            slicer.Refresh();
            // print: Alex
            //targetCell = ws.Cells[&quot;E1&quot;];
            Assert.AreEqual(&quot;Alex&quot;, targetCell.StringValue);

            // select all
            foreach (SlicerCacheItem cacheItem in slicer.SlicerCache.SlicerCacheItems)
            {
                cacheItem.Selected = true;
            }
            slicer.Refresh();
             targetCell = ws.Cells[&quot;E1&quot;];
            // print: Alex
            // expected: (All)
            Assert.AreEqual(&quot;(All)&quot;,targetCell.StringValue);
        }
```

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


