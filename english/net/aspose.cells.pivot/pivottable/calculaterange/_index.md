---
title: PivotTable.CalculateRange
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Calculates pivottables range
type: docs
url: /net/aspose.cells.pivot/pivottable/calculaterange/
---
## PivotTable.CalculateRange method

Calculates pivottable's range.

```csharp
public void CalculateRange()
```

### Remarks

If this method is not been called,maybe the pivottable range is not corrected.

### Examples

```csharp
// Called: t.CalculateRange();
private static void PivotTable_Method_CalculateRange(Workbook wb)
        {
            #region UPDATE pivot tables
            //Before the populated excel file is saved, calculate all pivot tables and charts.
            //Calculate formula has to be called before filtering to allow filters on calculated fields.
            wb.CalculateFormula();
            foreach (Worksheet sheet in wb.Worksheets)
            {
                foreach (Aspose.Cells.Pivot.PivotTable t in sheet.PivotTables)
                {
                    if (t.DataSource != null)
                    {
                        t.RefreshData();
                        //Range needs to be calculated before data is calculated to ensure that the record count is accounted for by the pivot table refresh.
                        t.CalculateRange();
                        t.CalculateData();
                        t.RefreshDataOnOpeningFile = true;
                    }
                    else
                    {
                        throw new Exception("The source data for the '" + t.Name + "' pivot table is missing. Please edit the report and reconnect the Pivot table to its data");
                    }
                }
            }
            wb.CalculateFormula();
            #endregion
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


