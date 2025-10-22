##Class FilterColumn
Aspose.Cells.FilterColumn class. Represents a filter for a single column. The Filter object is a member of the Filters collection
## FilterColumn class
Represents a filter for a single column. The Filter object is a member of the Filters collection
```csharp
public class FilterColumn
```
## Properties
| Name | Description |
| --- | --- |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | Gets and sets the column offset in the range. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | Gets and sets the condition of filtering data. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | Gets and sets the type fo filtering data. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | Indicates whether the AutoFilter button for this column is visible. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
namespace AsposeCellsExamples
{
public class FilterColumnDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["A2"].PutValue("John");
sheet.Cells["A3"].PutValue("Jane");
sheet.Cells["A4"].PutValue("Doe");
sheet.Cells["B1"].PutValue("Age");
sheet.Cells["B2"].PutValue(30);
sheet.Cells["B3"].PutValue(25);
sheet.Cells["B4"].PutValue(35);
// Apply AutoFilter to the range
sheet.AutoFilter.SetRange(0, 0, 3);
// Add a filter to the first column (Name)
sheet.AutoFilter.AddFilter(0, "John");
// Add a filter to the second column (Age)
sheet.AutoFilter.AddFilter(1, "30");
// Refresh the filter to apply it
sheet.AutoFilter.Refresh();
// Access the FilterColumnCollection
FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;
// Access the first FilterColumn
FilterColumn filterColumn = filterColumns[0];
// Display properties of the FilterColumn
Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
Console.WriteLine($"Filter: {filterColumn.Filter}");
Console.WriteLine($"FilterType: {filterColumn.FilterType}");
Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");
// Save the workbook
workbook.Save("FilterColumnDemo.xlsx");
workbook.Save("FilterColumnDemo.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
