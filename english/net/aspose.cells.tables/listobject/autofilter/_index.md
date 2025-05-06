---
title: ListObject.AutoFilter
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets auto filter
type: docs
url: /net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Gets auto filter.

```csharp
public AutoFilter AutoFilter { get; }
```

### Examples

```csharp
// Called: l.AutoFilter.Sorter.Sort();
private static void Property_AutoFilter(Workbook wb)
        {
            foreach (Worksheet wSheet in wb.Worksheets)
            {
                foreach (Aspose.Cells.Tables.ListObject l in wSheet.ListObjects)
                {
                    //Only attempt to clear the rest of the table if there is more to the table other than the first row.
                    if (l.DataRange.RowCount &gt; 1)
                    {
                        //Remove cells below the first datarow
                        wSheet.Cells.ClearContents(l.StartRow + 5, l.StartColumn, l.EndRow, l.EndColumn);
                        wSheet.Cells.ClearRange(l.StartRow + 5, l.StartColumn, l.EndRow, l.EndColumn);
                        wSheet.Cells.DeleteRange(l.StartRow + 5, l.StartColumn, l.EndRow, l.EndColumn, ShiftType.Up);
                    }

                    l.Resize(l.StartRow, l.StartColumn, l.StartRow + 4, l.EndColumn, true);

                    l.AutoFilter.Sorter.Sort();
                    l.AutoFilter.Refresh();
                }
            }
            wb.CalculateFormula();

            foreach (Worksheet wSheet in wb.Worksheets)
            {
                foreach (Aspose.Cells.Pivot.PivotTable pvt in wSheet.PivotTables)
                {
                    if (pvt.DataSource != null)
                    {
                        pvt.RefreshData();
                        pvt.CalculateData();
                        pvt.RefreshDataOnOpeningFile = false;
                    }
                }
            }
            wb.CalculateFormula();
        }
```

### See Also

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


