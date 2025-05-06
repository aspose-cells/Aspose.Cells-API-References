---
title: SlicerCacheItem.Value
second_title: Aspose.Cells for .NET API Reference
description: SlicerCacheItem property. Returns the label text for the slicer item. Readonly
type: docs
url: /net/aspose.cells.slicers/slicercacheitem/value/
---
## SlicerCacheItem.Value property

Returns the label text for the slicer item. Read-only.

```csharp
public string Value { get; }
```

### Examples

```csharp
// Called: cacheItem.Selected = cacheItem.Value == &amp;quot;Alex&amp;quot;;
[Test]
        public void Property_Value()
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

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


