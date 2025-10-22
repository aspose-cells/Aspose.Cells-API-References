##Row.FirstCell
Row property. Gets the first cell object in the row
## Row.FirstCell property
Gets the first cell object in the row.
```csharp
public Cell FirstCell { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyFirstCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add data to cells in first row
worksheet.Cells["A1"].PutValue("First Cell");
worksheet.Cells["B1"].PutValue("Second Cell");
worksheet.Cells["C1"].PutValue("Third Cell");
// Get the first row
Row row = worksheet.Cells.Rows[0];
// Demonstrate FirstCell property
Cell firstCell = row.FirstCell;
Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
// Modify the first cell
firstCell.PutValue("Modified First Cell");
Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
// Save the workbook
workbook.Save("RowFirstCellDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
