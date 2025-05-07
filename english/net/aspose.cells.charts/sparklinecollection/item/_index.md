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
// Called: Assert.AreEqual(workbook2.Worksheets[1].SparklineGroups[0].SparklineCollection[0].DataRange, "Sheet2!A2:D2");
[Test]
        public void Property_Int32_()
        {
            Workbook workbook1 = new Workbook(Constants.sourcePath + "CELLSJAVA41018.xlsx");
            Workbook workbook2 = new Workbook();

            workbook2.Combine(workbook1);
            Assert.AreEqual(workbook2.Worksheets[1].SparklineGroups[0].SparklineCollection[0].DataRange, "Sheet2!A2:D2");
        }
```

### See Also

* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


