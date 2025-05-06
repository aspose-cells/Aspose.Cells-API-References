---
title: Range.RowCount
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the count of rows in the range
type: docs
url: /net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Gets the count of rows in the range.

```csharp
public int RowCount { get; }
```

### Examples

```csharp
// Called: AssertHelper.checkCellArea(r.FirstRow, r.FirstColumn, r.FirstRow + r.RowCount - 1,
[Test]
        public void Property_RowCount()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            int p = 1;
            for (int i = 0; i &lt; 3; i++)
            {
                for (int j = 0; j &lt; 3; j++)
                {
                    cells[i, j].PutValue(p);
                    p &lt;&lt;= 1;
                }
            }
            string fml = &quot;Sheet1!$A$1:Sheet1!$A$1:$B$2:Sheet1!$C$3:Sheet1!$C$3&quot;;
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add(&quot;testname&quot;)];
            n.RefersTo = fml;
            Assert.AreEqual(&quot;=&quot; + fml, n.RefersTo, &quot;Name.RefersTo&quot;);
            Aspose.Cells.Range r = n.GetRange();
            AssertHelper.checkCellArea(r.FirstRow, r.FirstColumn, r.FirstRow + r.RowCount - 1,
                r.FirstColumn + r.ColumnCount - 1, CellArea.CreateCellArea(0, 0, 2, 2));
            Cell cell = cells[3, 0];
            fml = &quot;=SUM(&quot; + fml + &quot;)&quot;;
            cell.Formula = fml;
            Assert.AreEqual(fml, cell.Formula, &quot;Cell.Formula&quot;);
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual(511, cell.IntValue, &quot;Calculated result for multiple range operators&quot;);

            wb.Worksheets.Add();
            fml = &quot;=SUM(Sheet1:Sheet2!A2:B3:Sheet1:Sheet2!A3:C5)&quot;; //ms excel can set this formula, but calculate it as #VALUE!
            cell.Formula = fml;
            Assert.AreEqual(fml, cell.Formula, &quot;Cell.Formula&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


