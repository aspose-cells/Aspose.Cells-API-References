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
[Test]
        public void Property_EmptyFormulaValueAsBlank()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(&quot;a&quot;);
            cells[2, 2].PutValue(0);
            cells[4, 4].Formula = &quot;=B2&quot;;
            for (int i = 3; i &lt; 50; i++)
            {
                cells[i, 3].PutValue(&quot;&quot;);
            }

            Workbook wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankRows();
            Assert.AreEqual(2, cells.MaxRow, &quot;Normal1: MaxRow&quot;);

            wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyStringAsBlank = false });
            Assert.AreEqual(48, cells.MaxRow, &quot;EmptyStringAsBlank=false: MaxRow&quot;);

            cells = wb.Worksheets[0].Cells;
            cells[5, 5].SetDynamicArrayFormula(&quot;=D3:D50&quot;, new FormulaParseOptions(), true);
            cells[6, 6].Formula = &quot;=A1&quot;;
            wb.CalculateFormula();

            wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankRows();
            wbTest.RefreshDynamicArrayFormulas(true);
            Assert.AreEqual(50, cells.MaxRow, &quot;Normal2: MaxRow&quot;);
            Assert.IsTrue(cells[49, 5].IsDynamicArrayFormula, &quot;Normal2: F50.IsDynamicArrayFormula&quot;);
            Cell cell = cells.CheckCell(50, 5);
            Assert.IsTrue(cell == null || cell.Type == CellValueType.IsNull, &quot;Normal2: F51 should be blank&quot;);

            wbTest = new Workbook();
            wbTest.Copy(wb);
            cells = wbTest.Worksheets[0].Cells;
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            wbTest.RefreshDynamicArrayFormulas(true);
            Assert.AreEqual(6, cells.MaxRow, &quot;EmptyFormulaValueAsBlank: MaxRow&quot;);
            Assert.IsTrue(cells[6, 5].IsDynamicArrayFormula, &quot;EmptyFormulaValueAsBlank: F7.IsDynamicArrayFormula&quot;);
        }
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


