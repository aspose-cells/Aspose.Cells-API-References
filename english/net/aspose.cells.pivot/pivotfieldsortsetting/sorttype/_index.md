---
title: PivotFieldSortSetting.SortType
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldSortSetting property. Represents the SortOrder
type: docs
url: /net/aspose.cells.pivot/pivotfieldsortsetting/sorttype/
---
## PivotFieldSortSetting.SortType property

Represents the [`SortOrder`](../../../aspose.cells/sortorder/).

```csharp
public SortOrder SortType { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(SortOrder.Ascending, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.SortType);
[Test]
        public void Property_SortType()
        {
            var workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET46200_1.xlsx");
            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "K15");
          
            Assert.AreEqual("K15", workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.Cell);
            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "M15");
            Assert.AreEqual(SortOrder.Ascending, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.SortType);
            Assert.AreEqual("M15", workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.Cell);

            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "N15");
            Assert.AreEqual(PivotLineType.GrandTotal, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.LineTypeSortedBy);
            Assert.IsTrue(string.IsNullOrEmpty(workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.Cell));
        }
```

### See Also

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


