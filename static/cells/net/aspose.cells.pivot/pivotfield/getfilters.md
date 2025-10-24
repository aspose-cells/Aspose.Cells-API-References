##PivotField.GetFilters
PivotField method. Gets all pivot filters of this pivot field
## PivotField.GetFilters method
Gets all pivot filters of this pivot field.
```csharp
public PivotFilter[] GetFilters()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodGetFiltersDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Date";
worksheet.Cells["B1"].Value = "Sales";
for (int i = 2; i <= 10; i++)
{
worksheet.Cells[$"A{i}"].Value = DateTime.Now.AddDays(i-2);
worksheet.Cells[$"B{i}"].Value = i * 100;
}
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B10", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Apply date filter
PivotField dateField = pivotTable.RowFields[0];
DateTime startDate = DateTime.Now;
DateTime endDate = DateTime.Now.AddDays(5);
dateField.FilterByDate(PivotFilterType.DateBetween, startDate, endDate);
// Get and display filters
PivotFilter[] filters = dateField.GetFilters();
Console.WriteLine($"Number of filters applied: {filters.Length}");
if (filters.Length > 0)
{
Console.WriteLine($"Filter type: {filters[0].FilterType}");
Console.WriteLine($"Start date: {filters[0].GetDateTimeValues()[0]}");
Console.WriteLine($"End date: {filters[0].GetDateTimeValues()[1]}");
}
// Save the workbook
workbook.Save("PivotFieldGetFiltersDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../../pivotfilter/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
