---
title: Cell.IsInArray
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the cell formula is an array formula
type: docs
url: /net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

Indicates whether the cell formula is an array formula.

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.IsArrayFormula to check whether the cell formula is an array formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: if (!wSheet.Cells[l.StartRow + 1, i].IsFormula &amp;amp;&amp;amp; !wSheet.Cells[l.StartRow + 1, i].IsInArray)
private static void Property_IsInArray(Workbook wb)
        {
            foreach (Worksheet wSheet in wb.Worksheets)
            {
                foreach (Aspose.Cells.Tables.ListObject l in wSheet.ListObjects)
                {
                    //Set first data row values to sample values
                    for (int i = l.StartColumn; i &lt;= l.EndColumn; i++)
                    {
                        if (!wSheet.Cells[l.StartRow + 1, i].IsFormula &amp;&amp; !wSheet.Cells[l.StartRow + 1, i].IsInArray)
                        {
                            wSheet.Cells.ClearContents(l.StartRow + 1, i, l.StartRow + 1, i);
                            wSheet.Cells.ClearContents(l.StartRow + 2, i, l.StartRow + 2, i);
                        }
                    }

                    //Only attempt to clear the rest of the table if there is more to the table other than the first row.
                    if (l.DataRange.RowCount &gt; 2)
                    {
                        //Remove cells below the first datarow
                        wSheet.Cells.ClearContents(l.StartRow + 3, l.StartColumn, l.EndRow, l.EndColumn);
                        wSheet.Cells.ClearRange(l.StartRow + 3, l.StartColumn, l.EndRow, l.EndColumn);
                        wSheet.Cells.DeleteRange(l.StartRow + 3, l.StartColumn, l.EndRow, l.EndColumn, ShiftType.Up);
                    }

                    l.Resize(l.StartRow, l.StartColumn, l.StartRow + 2, l.EndColumn, true);

                    l.AutoFilter.Sorter.Sort();
                    l.AutoFilter.Refresh();
                }
            }
            wb.CalculateFormula();

            wb.Worksheets.RefreshPivotTables();
            wb.CalculateFormula();
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


