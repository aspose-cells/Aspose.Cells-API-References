---
title: Cells.MinColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Minimum column index of those cells that have been instantiated in the collectiondoes not include the column where style is defined for the whole column but no cell has been instantiated in it
type: docs
url: /net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

```csharp
public int MinColumn { get; }
```

### Examples

```csharp
// Called: int startColumn = Math.Min(cells1.MinColumn, cells2.MinColumn);
public void Cells_Property_MinColumn(Cells cells1, Cells cells2, string id1, string id2)
        {
            int endRow = Math.Max(cells1.MaxRow, cells2.MaxRow);
            int startColumn = Math.Min(cells1.MinColumn, cells2.MinColumn);
            int endColumn = Math.Max(cells1.MaxColumn, cells2.MaxColumn);
            for (int r = Math.Min(cells1.MinRow, cells2.MinRow); r <= endRow; r++)
            {
                for (int c = startColumn; c <= endColumn; c++)
                {
                    Cell cell1 = cells1.CheckCell(r, c);
                    Cell cell2 = cells2.CheckCell(r, c);
                    if (cell1 == null || IsNullCell(cell1))
                    {
                        if (cell2 == null || IsNullCell(cell2))
                        {
                            continue;
                        }
                        OnDifference(cell2.Name + ": " + id1 + " is empty but " + id2 + " is ["
                            + cell2.Type + "]" + cell2.Value);
                    }
                    else if (cell2 == null || IsNullCell(cell2))
                    {
                        OnDifference(cell1.Name + ": " + id1 + " is [" + cell1.Type + "]" + cell1.Value
                            + " but " + id2 + " is empty");
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
                                    OnDifference(cell1.Name + ": formula for " + id1 + " is "
                                        + fml1 + ", for " + id2 + " is " + fml2);
                                }
                            }
                            else
                            {
                                OnDifference(cell1.Name + ": " + id1 + " is formula but " + id2 + " is not");
                            }
                        }
                        else if (cell2.IsFormula)
                        {
                            OnDifference(cell1.Name + ": " + id1 + " is not formula but " + id2 + " is");
                        }
                        if (cell1.IsNumericValue)
                        {
                            if (cell2.IsNumericValue)
                            {
                                if (cell1.DoubleValue != cell2.DoubleValue)
                                {
                                    OnDifference(cell1.Name + ": [Numeric]" + id1 + " is " + cell1.DoubleValue
                                        + " but " + id2 + " is " + cell2.DoubleValue);
                                }
                            }
                            else
                            {
                                OnDifference(cell1.Name + ": " + id1 + " is [Numeric]" + cell1.DoubleValue
                                    + " but " + id2 + " is [" + cell2.Type + "]" + cell2.Value);
                            }
                        }
                        else if (cell2.IsNumericValue)
                        {
                            OnDifference(cell1.Name + ": " + id1 + " is [" + cell1.Type + "]" + cell1.Value
                                + " but " + id2 + " is [Numeric]" + cell2.DoubleValue);
                        }
                        else
                        {
                            CellValueType t1 = cell1.Type;
                            CellValueType t2 = cell2.Type;
                            if (t1 == t2)
                            {
                                if (!cell1.Value.Equals(cell2.Value))
                                {
                                    OnDifference(cell1.Name + ": [" + t1 + "]" + id1 + " is " + cell1.Value
                                        + " but " + id2 + " is " + cell2.Value);
                                }
                            }
                            else
                            {
                                OnDifference(cell1.Name + ": " + id1 + " is [" + cell1.Type + "]" + cell1.Value
                                    + " but " + id2 + " is [" + cell2.Type + "]" + cell2.Value);
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


