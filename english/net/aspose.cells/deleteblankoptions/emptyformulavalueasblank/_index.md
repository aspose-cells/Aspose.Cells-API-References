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
// Called: cells.DeleteBlankColumns(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
public void Property_EmptyFormulaValueAsBlank()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue("a");
            cells[2, 2].PutValue(0);
            cells[4, 4].Formula = "=B2";
            for (int i = 3; i < 50; i++)
            {
                cells[3, i].PutValue("");
            }

            Workbook wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankColumns();
            Assert.AreEqual(2, cells.MaxColumn, "Normal1: MaxColumn");

            wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankColumns(new DeleteBlankOptions() { EmptyStringAsBlank = false });
            Assert.AreEqual(48, cells.MaxColumn, "EmptyStringAsBlank=false: MaxColumn");

            cells = wb.Worksheets[0].Cells;
            cells[5, 5].SetDynamicArrayFormula("=C4:AX4", new FormulaParseOptions(), true);
            cells[6, 6].Formula = "=A1";
            wb.CalculateFormula();

            wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankColumns();
            wbTest.RefreshDynamicArrayFormulas(true);
            Assert.AreEqual(50, cells.MaxColumn, "Normal2: MaxColumn");
            Assert.IsTrue(cells[5, 49].IsDynamicArrayFormula, "Normal2: AX6.IsDynamicArrayFormula");
            Cell cell = cells.CheckCell(5, 50);
            Assert.IsTrue(cell == null || cell.Type == CellValueType.IsNull, "Normal2: AY6 should be blank");

            wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankColumns(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = false }); //CELLSNET-56865
            wbTest.RefreshDynamicArrayFormulas(true);
            Assert.AreEqual(50, cells.MaxColumn, "EmptyFormulaValueAsBlank=false: MaxColumn with default options instance");
            Assert.IsTrue(cells[5, 49].IsDynamicArrayFormula,
                "EmptyFormulaValueAsBlank=false: AX6.IsDynamicArrayFormula with default options instance");
            cell = cells.CheckCell(5, 50);
            Assert.IsTrue(cell == null || cell.Type == CellValueType.IsNull,
                "EmptyFormulaValueAsBlank=false: AY6 should be blank with default options instance");

            wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankColumns(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            wbTest.RefreshDynamicArrayFormulas(true);
            Assert.AreEqual(6, cells.MaxColumn, "EmptyFormulaValueAsBlank: MaxColumn");
            Assert.IsTrue(cells[5, 6].IsDynamicArrayFormula, "EmptyFormulaValueAsBlank: G6.IsDynamicArrayFormula");
        }
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


