---
title: LegendEntryCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: LegendEntryCollection property. Gets the LegendEntry element at the specified index
type: docs
url: /net/aspose.cells.charts/legendentrycollection/item/
---
## LegendEntryCollection indexer

Gets the [`LegendEntry`](../../legendentry/) element at the specified index.

```csharp
public LegendEntry this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[4].Charts[0].Legend.LegendEntries[3].IsDeleted, true);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41038.xlsx");
            workbook.Worksheets.AddCopy(0);
            Assert.AreEqual(workbook.Worksheets[4].Charts[0].Legend.LegendEntries[3].IsDeleted, true);
            Assert.AreEqual(workbook.Worksheets[4].Charts[0].CategoryAxis.MajorUnitScale, TimeUnit.Months);
        }
```

### See Also

* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


