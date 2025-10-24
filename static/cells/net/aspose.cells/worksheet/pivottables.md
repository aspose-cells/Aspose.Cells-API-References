##Worksheet.PivotTables
Worksheet property. Gets all pivot tables in this worksheet
## Worksheet.PivotTables property
Gets all pivot tables in this worksheet.
```csharp
public PivotTableCollection PivotTables { get; }
```
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class WorksheetPropertyPivotTablesDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("PivotTableExample.xlsx");
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access pivot tables collection from worksheet
PivotTableCollection pivotTables = worksheet.PivotTables;
// Check if there are any pivot tables
if (pivotTables.Count > 0)
{
// Get first pivot table
PivotTable pivotTable = pivotTables[0];
// Clear any existing filters
pivotTable.PivotFilters.Clear();
// Refresh pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the modified workbook
workbook.Save("PivotTableModified.xlsx");
}
}
}
}
```
### See Also
* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
