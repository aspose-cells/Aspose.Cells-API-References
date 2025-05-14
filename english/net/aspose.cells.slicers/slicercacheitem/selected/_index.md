---
title: SlicerCacheItem.Selected
second_title: Aspose.Cells for .NET API Reference
description: SlicerCacheItem property. Specifies whether the SlicerItem is selected or not
type: docs
url: /net/aspose.cells.slicers/slicercacheitem/selected/
---
## SlicerCacheItem.Selected property

Specifies whether the SlicerItem is selected or not.

```csharp
public bool Selected { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(slicerCacheItem.Selected);
public void SlicerCacheItem_Property_Selected()
{
    string[] files = new string[] { "example.xlsx", "example.xlsx" };
    for(int j = 0; j < files.Length;j++)
    {
        Workbook workbook = new Workbook(Constants.PivotTableSourcePath + files[j]);
        workbook.Worksheets.RefreshAll();
        var slicer = workbook.Worksheets
                .SelectMany(x => x.Slicers)
                .First();

        for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
        {
            SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
            if (i == 0)
                Assert.IsTrue(slicerCacheItem.Selected);
            else
            {
                Assert.IsFalse(slicerCacheItem.Selected);
            }
        }
        workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
    }
          
}
```

### See Also

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


