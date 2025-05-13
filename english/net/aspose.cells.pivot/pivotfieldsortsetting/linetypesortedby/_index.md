---
title: PivotFieldSortSetting.LineTypeSortedBy
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldSortSetting property. The pivot line type sorted by
type: docs
url: /net/aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/
---
## PivotFieldSortSetting.LineTypeSortedBy property

The pivot line type sorted by.

```csharp
public PivotLineType LineTypeSortedBy { get; }
```

### Remarks

Only works when not sorting this field by labels.

### Examples

```csharp
// Called: Assert.AreEqual(PivotLineType.GrandTotal, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.LineTypeSortedBy);
public void PivotFieldSortSetting_Property_LineTypeSortedBy()
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

* enum [PivotLineType](../../pivotlinetype/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


