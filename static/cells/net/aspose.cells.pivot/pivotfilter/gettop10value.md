##PivotFilter.GetTop10Value
PivotFilter method. Gets top 10 setting of the filter
## PivotFilter.GetTop10Value method
Gets top 10 setting of the filter.
```csharp
public Top10Filter GetTop10Value()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterMethodGetTop10ValueDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Access first worksheet and pivot table
Worksheet worksheet = workbook.Worksheets[0];
PivotTable pivotTable = worksheet.PivotTables[0];
// Apply top 10 filter on first base field (show top 2 items by count)
pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
// Get the applied filter and its top 10 value
PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
Top10Filter top10Filter = filter.GetTop10Value();
// Output the filter details
Console.WriteLine("Filter Type: " + filter.FilterType);
Console.WriteLine("Top 10 Items: " + top10Filter.Items);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
