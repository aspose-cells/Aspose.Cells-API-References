---
title: PivotTable.ShowColumnGrandTotals
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether to show grand totals for columns of this pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/showcolumngrandtotals/
---
## PivotTable.ShowColumnGrandTotals property

Indicates whether to show grand totals for columns of this pivot table.

```csharp
public bool ShowColumnGrandTotals { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets[0].PivotTables[0].ShowColumnGrandTotals);
public void PivotTable_Property_ShowColumnGrandTotals()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].ShowRowGrandTotals);
    Assert.IsFalse(workbook.Worksheets[0].PivotTables[0].ShowColumnGrandTotals);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].ShowRowGrandTotals);
    Assert.IsFalse(workbook.Worksheets[0].PivotTables[0].ShowColumnGrandTotals);
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].ShowRowGrandTotals);
    Assert.IsFalse(workbook.Worksheets[0].PivotTables[0].ShowColumnGrandTotals);
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].ShowRowGrandTotals);
    Assert.IsFalse(workbook.Worksheets[0].PivotTables[0].ShowColumnGrandTotals);
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


