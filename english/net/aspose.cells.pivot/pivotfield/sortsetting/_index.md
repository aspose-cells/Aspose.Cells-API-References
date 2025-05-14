---
title: PivotField.SortSetting
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets all settings of auto sorting
type: docs
url: /net/aspose.cells.pivot/pivotfield/sortsetting/
---
## PivotField.SortSetting property

Gets all settings of auto sorting

```csharp
public PivotFieldSortSetting SortSetting { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(PivotLineType.GrandTotal, workbook.Worksheets[0].PivotTables[0].RowFields[0].SortSetting.LineTypeSortedBy);
public void PivotField_Property_SortSetting()
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

* class [PivotFieldSortSetting](../../pivotfieldsortsetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


