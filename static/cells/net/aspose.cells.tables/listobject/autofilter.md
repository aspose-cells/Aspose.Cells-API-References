##ListObject.AutoFilter
ListObject property. Gets auto filter
## ListObject.AutoFilter property
Gets auto filter.
```csharp
public AutoFilter AutoFilter { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyAutoFilterDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Mary");
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["A4"].PutValue("Peter");
worksheet.Cells["B4"].PutValue(35);
// Create a ListObject
int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
ListObject listObject = worksheet.ListObjects[index];
// Resize the list object to include all data
listObject.Resize(0, 0, 4, 2, true);
// Access and demonstrate AutoFilter functionality
if (listObject.AutoFilter != null)
{
// Apply filter on Age column (column 2)
listObject.AutoFilter.Filter(1, "25");
// Show filtered data
Console.WriteLine("Filtered Data:");
for (int row = 1; row <= 4; row++)
{
if (!worksheet.Cells.Rows[row].IsHidden)
{
Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
}
}
// Clear the filter
listObject.AutoFilter.RemoveFilter(1);
}
// Save the workbook
workbook.Save("ListObjectAutoFilterDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
