---
title: Cell.IsFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents if the specified cell contains formula
type: docs
url: /net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Represents if the specified cell contains formula.

```csharp
public bool IsFormula { get; }
```

### Examples

```csharp
// Called: else if (cell != null &amp;amp;&amp;amp; (cell.IsFormula || cell.Type != CellValueType.IsNull))
private void Property_IsFormula(Cells cells, string fml, int recs, int cols, string msgHeader)
        {
            double v = (int)CellsHelper.GetDoubleFromDateTime(new DateTime(2022, 8, 13), false);
            for (int i = recs + 5; i&gt;-1; i--)
            {
                for (int j = 0; j &lt; cols; j++)
                {
                    Cell cell = cells.CheckCell(i, j);
                    if (i &lt; recs)
                    {
                        if (cell == null)
                        {
                            Assert.Fail(msgHeader + CellsHelper.CellIndexToName(i, j)
                                + &quot; should be spilled with dynamic formula but was not&quot;);
                        }
                        Assert.AreEqual(fml, cell.Formula, msgHeader + cell.Name);
                        Assert.AreEqual(j == 0 ? v + i : 100.0 + i / 10.0, cell.DoubleValue, msgHeader + cell.Name);
                    }
                    else if (cell != null &amp;&amp; (cell.IsFormula || cell.Type != CellValueType.IsNull))
                    {
                        Assert.Fail(msgHeader + cell + &quot; should be empty&quot;);
                    }
                }
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


