##Row.LastCell
Row property. Gets the last cell object in the row
## Row.LastCell property
Gets the last cell object in the row.
```csharp
public Cell LastCell { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyLastCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("First");
worksheet.Cells["B1"].PutValue("Second");
worksheet.Cells["C1"].PutValue("Last");
// Get the first row
Row row = worksheet.Cells.Rows[0];
// Access the last cell in the row
Cell lastCell = row.LastCell;
// Output the value of the last cell
Console.WriteLine("Last cell value: " + lastCell.Value);
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
