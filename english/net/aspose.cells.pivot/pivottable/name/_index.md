---
title: PivotTable.Name
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the name of the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/name/
---
## PivotTable.Name property

Gets the name of the PivotTable

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: throw new Exception("The source data for the '" + t.Name + "' pivot table is missing. Please edit the report and reconnect the Pivot table to its data");
private static void PivotTable_Property_Name(Workbook wb)
        {
            #region UPDATE pivot tables
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
            #endregion
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


