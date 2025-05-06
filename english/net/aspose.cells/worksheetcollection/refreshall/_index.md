---
title: WorksheetCollection.RefreshAll
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Refresh all pivot tables and charts with pivot source
type: docs
url: /net/aspose.cells/worksheetcollection/refreshall/
---
## WorksheetCollection.RefreshAll method

Refresh all pivot tables and charts with pivot source.

```csharp
public void RefreshAll()
```

### Examples

```csharp
// Called: workbook.Worksheets.RefreshAll();
[Test]
        public void Method_RefreshAll()
        {
            string[] files = new string[] { &quot;CELLSNET56535.xlsx&quot;, &quot;CELLSNET56535_2.xlsx&quot; };
            for(int j = 0; j &lt; files.Length;j++)
            {
                Workbook workbook = new Workbook(Constants.PivotTableSourcePath + files[j]);
                workbook.Worksheets.RefreshAll();
                var slicer = workbook.Worksheets
                        .SelectMany(x =&gt; x.Slicers)
                        .First();

                for (int i = 0; i &lt; slicer.SlicerCache.SlicerCacheItems.Count; i++)
                {
                    SlicerCacheItem slicerCacheItem = slicer.SlicerCache.SlicerCacheItems[i];
                    if (i == 0)
                        Assert.IsTrue(slicerCacheItem.Selected);
                    else
                    {
                        Assert.IsFalse(slicerCacheItem.Selected);
                    }
                }
                workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET56535.xlsx&quot;);
            }
          
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


