##FilterColumn.FilterType
FilterColumn property. Gets and sets the type fo filtering data
## FilterColumn.FilterType property
Gets and sets the type fo filtering data.
```csharp
public FilterType FilterType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FilterColumnPropertyFilterTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Department");
sheet.Cells["A2"].PutValue("HR");
sheet.Cells["A3"].PutValue("IT");
sheet.Cells["A4"].PutValue("Finance");
sheet.Cells["B1"].PutValue("Employees");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(15);
sheet.Cells["B4"].PutValue(8);
// Apply auto filter using string range
sheet.AutoFilter.Range = "A1:B4";
// Add different filter types to demonstrate FilterType property
sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter
// Get filter columns
FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;
// Display FilterType for each column
for (int i = 0; i < filterColumns.Count; i++)
{
FilterColumn filterColumn = filterColumns[i];
Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
}
// Save the workbook
workbook.Save("FilterTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
