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
// Called: SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
public void Slicers_Type_SlicerCacheItem()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    workbook.Worksheets.RefreshAll();
    var slicer = workbook.Worksheets
            .SelectMany(x => x.Slicers)
            .First();

    for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
    {
        SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
        Assert.IsTrue(slicerCacheItem.Selected);
    }
}
```

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


