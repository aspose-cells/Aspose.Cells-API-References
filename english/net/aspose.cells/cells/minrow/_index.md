---
title: Cells.MinRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Minimum row index of cell which contains data or style
type: docs
url: /net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Minimum row index of cell which contains data or style.

```csharp
public int MinRow { get; }
```

### Examples

```csharp
// Called: for (int r = Math.Min(cells1.MinRow, cells2.MinRow); r &amp;lt;= endRow; r++)
public void Property_MinRow(Cells cells1, Cells cells2, string id1, string id2)
        {
            int endRow = Math.Max(cells1.MaxRow, cells2.MaxRow);
            int startColumn = Math.Min(cells1.MinColumn, cells2.MinColumn);
            int endColumn = Math.Max(cells1.MaxColumn, cells2.MaxColumn);
            for (int r = Math.Min(cells1.MinRow, cells2.MinRow); r &lt;= endRow; r++)
            {
                for (int c = startColumn; c &lt;= endColumn; c++)
                {
                    Cell cell1 = cells1.CheckCell(r, c);
                    Cell cell2 = cells2.CheckCell(r, c);
                    if (cell1 == null || IsNullCell(cell1))
                    {
                        if (cell2 == null || IsNullCell(cell2))
                        {
                            continue;
                        }
                        OnDifference(cell2.Name + &quot;: &quot; + id1 + &quot; is empty but &quot; + id2 + &quot; is [&quot;
                            + cell2.Type + &quot;]&quot; + cell2.Value);
                    }
                    else if (cell2 == null || IsNullCell(cell2))
                    {
                        OnDifference(cell1.Name + &quot;: &quot; + id1 + &quot; is [&quot; + cell1.Type + &quot;]&quot; + cell1.Value
                            + &quot; but &quot; + id2 + &quot; is empty&quot;);
                    }
                    else
                    {
                        if (cell1.IsFormula)
                        {
                            if (cell2.IsFormula)
                            {
                                string fml1 = cell1.Formula;
                                string fml2 = cell2.Formula;
                                if (fml1 != fml2)
                                {
                                    OnDifference(cell1.Name + &quot;: formula for &quot; + id1 + &quot; is &quot;
                                        + fml1 + &quot;, for &quot; + id2 + &quot; is &quot; + fml2);
                                }
                            }
                            else
                            {
                                OnDifference(cell1.Name + &quot;: &quot; + id1 + &quot; is formula but &quot; + id2 + &quot; is not&quot;);
                            }
                        }
                        else if (cell2.IsFormula)
                        {
                            OnDifference(cell1.Name + &quot;: &quot; + id1 + &quot; is not formula but &quot; + id2 + &quot; is&quot;);
                        }
                        if (cell1.IsNumericValue)
                        {
                            if (cell2.IsNumericValue)
                            {
                                if (cell1.DoubleValue != cell2.DoubleValue)
                                {
                                    OnDifference(cell1.Name + &quot;: [Numeric]&quot; + id1 + &quot; is &quot; + cell1.DoubleValue
                                        + &quot; but &quot; + id2 + &quot; is &quot; + cell2.DoubleValue);
                                }
                            }
                            else
                            {
                                OnDifference(cell1.Name + &quot;: &quot; + id1 + &quot; is [Numeric]&quot; + cell1.DoubleValue
                                    + &quot; but &quot; + id2 + &quot; is [&quot; + cell2.Type + &quot;]&quot; + cell2.Value);
                            }
                        }
                        else if (cell2.IsNumericValue)
                        {
                            OnDifference(cell1.Name + &quot;: &quot; + id1 + &quot; is [&quot; + cell1.Type + &quot;]&quot; + cell1.Value
                                + &quot; but &quot; + id2 + &quot; is [Numeric]&quot; + cell2.DoubleValue);
                        }
                        else
                        {
                            CellValueType t1 = cell1.Type;
                            CellValueType t2 = cell2.Type;
                            if (t1 == t2)
                            {
                                if (!cell1.Value.Equals(cell2.Value))
                                {
                                    OnDifference(cell1.Name + &quot;: [&quot; + t1 + &quot;]&quot; + id1 + &quot; is &quot; + cell1.Value
                                        + &quot; but &quot; + id2 + &quot; is &quot; + cell2.Value);
                                }
                            }
                            else
                            {
                                OnDifference(cell1.Name + &quot;: &quot; + id1 + &quot; is [&quot; + cell1.Type + &quot;]&quot; + cell1.Value
                                    + &quot; but &quot; + id2 + &quot; is [&quot; + cell2.Type + &quot;]&quot; + cell2.Value);
                            }
                        }
                    }
                }
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


