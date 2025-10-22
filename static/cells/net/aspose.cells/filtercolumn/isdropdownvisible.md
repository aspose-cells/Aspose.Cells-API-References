##FilterColumn.IsDropdownVisible
FilterColumn property. Indicates whether the AutoFilter button for this column is visible
## FilterColumn.IsDropdownVisible property
Indicates whether the AutoFilter button for this column is visible.
```csharp
public bool IsDropdownVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FilterColumnPropertyIsDropdownVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("Fruit");
sheet.Cells["A3"].PutValue("Vegetable");
sheet.Cells["A4"].PutValue("Fruit");
// Apply AutoFilter
sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string
// Get the filter column
FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];
// Show dropdown initially
filterColumn.IsDropdownVisible = true;
Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");
// Hide the dropdown
filterColumn.IsDropdownVisible = false;
Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");
// Save the workbook
workbook.Save("FilterColumnDropdownDemo.xlsx");
}
}
}
```
### See Also
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
