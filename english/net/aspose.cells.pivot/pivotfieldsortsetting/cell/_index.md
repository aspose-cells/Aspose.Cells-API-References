---
title: PivotFieldSortSetting.Cell
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldSortSetting property. Sorts by the values in which row or column
type: docs
url: /net/aspose.cells.pivot/pivotfieldsortsetting/cell/
---
## PivotFieldSortSetting.Cell property

Sorts by the values in which row or column.

```csharp
public string Cell { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("K15", workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.Cell);
public void PivotFieldSortSetting_Property_Cell()
{
    var workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
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

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


