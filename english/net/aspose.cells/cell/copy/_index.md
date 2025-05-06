---
title: Cell.Copy
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Copies data from a source cell
type: docs
url: /net/aspose.cells/cell/copy/
---
## Cell.Copy method

Copies data from a source cell.

```csharp
public void Copy(Cell cell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Source [`Cell`](../) object. |

### Examples

```csharp
// Called: b2.Copy(b1);
[Test]
        public void Method_Cell_()
        {
            Workbook wb = new Workbook();
            wb.Settings.FormulaSettings.EnableCalculationChain = true;
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(1);
            cells[1, 0].PutValue(2);
            cells[2, 0].PutValue(4);
            cells[0, 1].Formula = &quot;=SUM(A1:A2)&quot;;
            cells[0, 2].Formula = &quot;=B1+1&quot;;
            wb.CalculateFormula();
            Assert.AreEqual(4, cells[0, 2].IntValue, &quot;First calculation&quot;);
            wb.CalculateFormula();
            Assert.AreEqual(4, cells[0, 2].IntValue, &quot;Second calculation&quot;);
            Cell b1 = cells[0, 1];
            Cell b2 = cells[1, 1];
            b2.Copy(b1);
            wb.CalculateFormula();
            Assert.AreEqual(6, b2.IntValue, &quot;After Cell.Copy(), B2.Value&quot;);
            b1.Formula = &quot;=SUM(A1:A3)&quot;;
            wb.CalculateFormula();
            Assert.AreEqual(7, b1.IntValue, &quot;After resetting formula, B2.Value&quot;);

            DataTable dataTable = new DataTable();
            dataTable.Columns.Add(new DataColumn(&quot;A&quot;, typeof(int)));
            dataTable.Rows.Add(-1);
            dataTable.Rows.Add(-2);
            dataTable.Rows.Add(-4);
            cells.ImportData(dataTable, 0, 0, new ImportTableOptions() { InsertRows = false, IsFieldNameShown = false });
            wb.CalculateFormula();
            Assert.AreEqual(-7, b1.IntValue, &quot;After Cells.ImportData(), B1.Value&quot;);
            Assert.AreEqual(-6, b2.IntValue, &quot;After Cells.ImportData(), B2.Value&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


