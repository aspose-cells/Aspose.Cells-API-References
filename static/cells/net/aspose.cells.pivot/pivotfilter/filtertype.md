##PivotFilter.FilterType
PivotFilter property. Gets the autofilter type of the pivot filter
## PivotFilter.FilterType property
Gets the autofilter type of the pivot filter.
```csharp
public PivotFilterType FilterType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyFilterTypeDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Access first worksheet and pivot table
Worksheet worksheet = workbook.Worksheets[0];
PivotTable pivotTable = worksheet.PivotTables[0];
// Apply value filter (less than 2) to first base field
pivotTable.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
// Save the workbook
workbook.Save("output.xlsx");
// Reload the workbook to verify the filter
Workbook verifyWorkbook = new Workbook("output.xlsx");
PivotTable verifyPivotTable = verifyWorkbook.Worksheets[0].PivotTables[0];
// Get the applied filter and demonstrate FilterType property
PivotFilter filter = verifyPivotTable.BaseFields[0].GetFilters()[0];
Console.WriteLine("Filter Type: " + filter.FilterType); // Should output ValueLessThan
Console.WriteLine("Filter Value: " + filter.GetNumberValues()[0]); // Should output 2
}
}
}
```
### See Also
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
