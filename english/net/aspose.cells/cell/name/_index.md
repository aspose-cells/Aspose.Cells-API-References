---
title: Cell.Name
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the name of the cell
type: docs
url: /net/aspose.cells/cell/name/
---
## Cell.Name property

Gets the name of the cell.

```csharp
public string Name { get; }
```

### Remarks

A cell name includes its column letter and row number. For example, the name of a cell in row 0 and column 0 is A1.

### Examples

```csharp
// Called: string cn = cell.Name;
[Test]
        public void Property_Name()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].SetDynamicArrayFormula(&quot;={1,2,3;4,5,6;7,8,9}&quot;, new FormulaParseOptions(), true);
            wb.Worksheets.Names[wb.Worksheets.Names.Add(&quot;testspilledref&quot;)].RefersTo = &quot;Sheet1!$A$1#&quot;;
            cells[0, 5].SetDynamicArrayFormula(&quot;=-A1#&quot;, new FormulaParseOptions(), true);
            cells[4, 5].SetDynamicArrayFormula(&quot;=testspilledref&quot;, new FormulaParseOptions(), true);
            Cell cell;
            for (int i = 0; i &lt; 3; i++)
            {
                for (int j = 0; j &lt; 3; j++)
                {
                    int v = i * 3 + j + 1;
                    cell = cells[i, j];
                    string cn = cell.Name;
                    Assert.AreEqual(&quot;={1,2,3;4,5,6;7,8,9}&quot;, cell.Formula, cn);
                    Assert.AreEqual(v, cell.IntValue, cn);
                    cell = cells[i, j + 5];
                    cn = cell.Name;
                    Assert.AreEqual(&quot;=-A1#&quot;, cell.Formula, cn);
                    Assert.AreEqual(-v, cell.IntValue, cn);
                    cell = cells[i + 4, j + 5];
                    cn = cell.Name;
                    Assert.AreEqual(&quot;=testspilledref&quot;, cell.Formula, cn);
                    Assert.AreEqual(v, cell.IntValue, cn);
                }
            }
            cells[0, 0].SetDynamicArrayFormula(&quot;={11,12;13,14}&quot;, new FormulaParseOptions(), true);
            wb.RefreshDynamicArrayFormulas(true);
            for (int i = 0; i &lt; 3; i++)
            {
                for (int j = 0; j &lt; 3; j++)
                {
                    if (i &gt; 1 || j &gt; 1)
                    {
                        cell = cells.CheckCell(i, j);
                        if (cell != null &amp;&amp; (cell.Formula != null || cell.Value != null))
                        {
                            Assert.Fail(cell.Name + &quot; should be empty&quot;);
                        }
                        continue;
                    }
                    int v = i * 2 + j + 11;
                    cell = cells[i, j];
                    string cn = cell.Name;
                    Assert.AreEqual(&quot;={11,12;13,14}&quot;, cell.Formula, cn);
                    Assert.AreEqual(v, cell.IntValue, cn);
                    cell = cells[i, j + 5];
                    cn = cell.Name;
                    Assert.AreEqual(&quot;=-A1#&quot;, cell.Formula, cn);
                    Assert.AreEqual(-v, cell.IntValue, cn);
                    cell = cells[i + 4, j + 5];
                    cn = cell.Name;
                    Assert.AreEqual(&quot;=testspilledref&quot;, cell.Formula, cn);
                    Assert.AreEqual(v, cell.IntValue, cn);
                }
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


