---
title: SparklineCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: SparklineCollection property. Gets the Sparkline element at the specified index
type: docs
url: /net/aspose.cells.charts/sparklinecollection/item/
---
## SparklineCollection indexer

Gets the [`Sparkline`](../../sparkline/) element at the specified index.

```csharp
public Sparkline this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual("Sheet1!A1:D1", sparklineGroups[0].Sparklines[0].DataRange);
public void SparklineCollection_Property_Item()
{
    Workbook source = new Workbook(Constants.sourcePath + "example.xlsx");


    source.Save(Constants.destPath + "example.ods");
    source = new Workbook(Constants.destPath + "example.ods");
    SparklineGroupCollection sparklineGroups = source.Worksheets[0].SparklineGroups;
    Assert.AreEqual(3, sparklineGroups.Count);
    Assert.AreEqual(SparklineType.Line, sparklineGroups[0].Type);
    Assert.AreEqual("Sheet1!A1:D1", sparklineGroups[0].Sparklines[0].DataRange);
    Assert.AreEqual(SparklineType.Column,sparklineGroups[1].Type);
    Assert.AreEqual(SparklineType.Stacked, sparklineGroups[2].Type);
    source.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


