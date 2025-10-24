##Row.IsCollapsed
Row property. whether the row is collapsed
## Row.IsCollapsed property
whether the row is collapsed
```csharp
public bool IsCollapsed { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyIsCollapsedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create and style a row
Row row = worksheet.Cells.Rows[0];
row.Height = 20;
row.GroupLevel = 1;
// Demonstrate IsCollapsed property
row.IsCollapsed = true;
Console.WriteLine("Row is collapsed: " + row.IsCollapsed);
// Expand the row
row.IsCollapsed = false;
Console.WriteLine("Row is collapsed: " + row.IsCollapsed);
// Save the workbook
workbook.Save("RowIsCollapsedDemo.xlsx");
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
