---
title: DeleteBlankOptions.EmptyFormulaValueAsBlank
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false
type: docs
url: /net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Remarks

Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [`Formula`](../../cell/formula/) will be taken as blank and may be deleted because before calculation their calculated results are all null.

### Examples

```csharp
// Called: cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
public void DeleteBlankOptions_Property_EmptyFormulaValueAsBlank()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells[0, 0].PutValue("a");
    cells[2, 2].PutValue(0);
    cells[4, 4].Formula = "=B2";
    for (int i = 3; i < 50; i++)
    {
        cells[i, 3].PutValue("");
    }

    Workbook wbTest = new Workbook();
    wbTest.Copy(wb);
    cells = wbTest.Worksheets[0].Cells;
    cells.DeleteBlankRows();
    Assert.AreEqual(2, cells.MaxRow, "Normal1: MaxRow");

    wbTest = new Workbook();
    wbTest.Copy(wb);
    cells = wbTest.Worksheets[0].Cells;
    cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyStringAsBlank = false });
    Assert.AreEqual(48, cells.MaxRow, "EmptyStringAsBlank=false: MaxRow");

    cells = wb.Worksheets[0].Cells;
    cells[5, 5].SetDynamicArrayFormula("=D3:D50", new FormulaParseOptions(), true);
    cells[6, 6].Formula = "=A1";
    wb.CalculateFormula();

    wbTest = new Workbook();
    wbTest.Copy(wb);
    cells = wbTest.Worksheets[0].Cells;
    cells.DeleteBlankRows();
    wbTest.RefreshDynamicArrayFormulas(true);
    Assert.AreEqual(50, cells.MaxRow, "Normal2: MaxRow");
    Assert.IsTrue(cells[49, 5].IsDynamicArrayFormula, "Normal2: F50.IsDynamicArrayFormula");
    Cell cell = cells.CheckCell(50, 5);
    Assert.IsTrue(cell == null || cell.Type == CellValueType.IsNull, "Normal2: F51 should be blank");

    wbTest = new Workbook();
    wbTest.Copy(wb);
    cells = wbTest.Worksheets[0].Cells;
    cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
    wbTest.RefreshDynamicArrayFormulas(true);
    Assert.AreEqual(6, cells.MaxRow, "EmptyFormulaValueAsBlank: MaxRow");
    Assert.IsTrue(cells[6, 5].IsDynamicArrayFormula, "EmptyFormulaValueAsBlank: F7.IsDynamicArrayFormula");
}
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


