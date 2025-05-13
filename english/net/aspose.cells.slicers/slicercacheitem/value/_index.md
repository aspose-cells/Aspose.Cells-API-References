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
// Called: cacheItem.Selected = cacheItem.Value == "Alex";
public void SlicerCacheItem_Property_Value()
{
    var wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    var ws = wb.Worksheets[0];
    ws.RefreshPivotTables();

    var targetCell = ws.Cells["E1"];
    // print: (All)
    Console.WriteLine(targetCell.Value);

    var slicer = ws.Slicers[0];
    // select alex
    foreach (SlicerCacheItem cacheItem in slicer.SlicerCache.SlicerCacheItems)
    {
        cacheItem.Selected = cacheItem.Value == "Alex";
    }
    slicer.Refresh();
    // print: Alex
    //targetCell = ws.Cells["E1"];
    Assert.AreEqual("Alex", targetCell.StringValue);

    // select all
    foreach (SlicerCacheItem cacheItem in slicer.SlicerCache.SlicerCacheItems)
    {
        cacheItem.Selected = true;
    }
    slicer.Refresh();
     targetCell = ws.Cells["E1"];
    // print: Alex
    // expected: (All)
    Assert.AreEqual("(All)",targetCell.StringValue);
}
```

### See Also

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


