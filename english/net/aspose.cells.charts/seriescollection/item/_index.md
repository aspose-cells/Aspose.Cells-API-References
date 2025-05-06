---
title: SeriesCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection property. Gets the Series element at the specified index
type: docs
url: /net/aspose.cells.charts/seriescollection/item/
---
## SeriesCollection indexer

Gets the [`Series`](../../series/) element at the specified index.

```csharp
public Series this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets[1].Charts[0].NSeries[0].Values, &amp;quot;=Sheet4!$C$2:$C$405&amp;quot;);
[Test]
        public void Property_Int32_()
        {
            Aspose.Cells.Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet44465.xlsx&quot;);
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            foreach (Worksheet sheet in wb.Worksheets)
            {
                sheet.Cells.DeleteBlankColumns(options);
                sheet.Cells.DeleteBlankRows(options);
            }
            Assert.AreEqual(wb.Worksheets[1].Charts[0].NSeries[0].Values, &quot;=Sheet4!$C$2:$C$405&quot;);
        }
```

### See Also

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


