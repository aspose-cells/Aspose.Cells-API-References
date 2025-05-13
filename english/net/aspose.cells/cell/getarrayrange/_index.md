---
title: Cell.GetArrayRange
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the array range if the cells formula is an array formula
type: docs
url: /net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Gets the array range if the cell's formula is an array formula.

```csharp
public CellArea GetArrayRange()
```

### Return Value

The array range.

### Remarks

Only applies when the cell's formula is an array formula

### Examples

```csharp
// Called: AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + ".ArrayRange");
public void Cell_Method_GetArrayRange()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    string fml = "=MAP(SEQUENCE(10), LAMBDA(x, SUM(MAP(SEQUENCE(x), LAMBDA(x, x * x)))))";
    cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), false);
    wb.CalculateFormula();
    CellArea expected = CellArea.CreateCellArea(0, 0, 9, 0);
    AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + ".ArrayRange");
    DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, "");
    DynamicFormulaTest.CheckResult(
        new string[] { "1", "5", "14", "30", "55", "91", "140", "204", "285", "385", },
        cells, expected, fml);

    fml = "=MAP(SEQUENCE(10), LAMBDA(x, SUM(MAP(MAP(SEQUENCE(x), LAMBDA(y, y * y)), LAMBDA(y, y+1)))))";
    cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
    AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + ".ArrayRange");
    DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, "");
    DynamicFormulaTest.CheckResult(
        new string[] { "2", "7", "17", "34", "60", "97", "147", "212", "294", "395", },
        cells, expected, fml);
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


