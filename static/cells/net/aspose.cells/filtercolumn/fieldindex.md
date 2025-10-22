##FilterColumn.FieldIndex
FilterColumn property. Gets and sets the column offset in the range
## FilterColumn.FieldIndex property
Gets and sets the column offset in the range.
```csharp
public int FieldIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FilterColumnPropertyFieldIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Department");
worksheet.Cells["B1"].PutValue("Employees");
worksheet.Cells["A2"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(15);
worksheet.Cells["A3"].PutValue("Marketing");
worksheet.Cells["B3"].PutValue(8);
worksheet.Cells["A4"].PutValue("IT");
worksheet.Cells["B4"].PutValue(12);
// Apply auto filter
worksheet.AutoFilter.Range = "A1:B4";
// Add filter to first column (Department)
worksheet.AutoFilter.AddFilter(0, "Sales");
// Get the filter column
FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
// Demonstrate FieldIndex property
Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
// Refresh and save
worksheet.AutoFilter.Refresh();
workbook.Save("FilterColumnFieldIndexDemo.xlsx");
}
}
}
```
### See Also
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
