---
title: PivotItemCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: PivotItemCollection property. Gets the count of the pivot items
type: docs
url: /net/aspose.cells.pivot/pivotitemcollection/count/
---
## PivotItemCollection.Count property

Gets the count of the pivot items.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2, workbook.Worksheets[0].PivotTables[0].RowFields[0].PivotItems.Count);
[Test]
        public void Property_Count()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET55447.xlsx");
            Assert.AreEqual(2, workbook.Worksheets[0].PivotTables[0].RowFields[0].PivotItems.Count);
        }
```

### See Also

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


