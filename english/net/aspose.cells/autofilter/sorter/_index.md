---
title: AutoFilter.Sorter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter property. Gets the data sorter
type: docs
url: /net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Gets the data sorter.

```csharp
public DataSorter Sorter { get; }
```

### Examples

```csharp
// Called: l.AutoFilter.Sorter.Sort();
private static void Property_Sorter(Workbook wb)
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

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


