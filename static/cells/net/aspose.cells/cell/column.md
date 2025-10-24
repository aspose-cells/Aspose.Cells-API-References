##Cell.Column
Cell property. Gets column number zero based of the cell
## Cell.Column property
Gets column number (zero based) of the cell.
```csharp
public int Column { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cells and demonstrate Column property
Cell cell1 = worksheet.Cells["A1"];
Cell cell2 = worksheet.Cells["B2"];
Cell cell3 = worksheet.Cells["C3"];
// Set values and styles
cell1.PutValue("Cell A1");
cell2.PutValue("Cell B2");
cell3.PutValue("Cell C3");
// Demonstrate Column property usage
Console.WriteLine("Cell A1 is in column: " + cell1.Column);
Console.WriteLine("Cell B2 is in column: " + cell2.Column);
Console.WriteLine("Cell C3 is in column: " + cell3.Column);
// Modify column width using Column property
worksheet.Cells.Columns[cell1.Column].Width = 20;
worksheet.Cells.Columns[cell2.Column].Width = 25;
worksheet.Cells.Columns[cell3.Column].Width = 30;
// Save the workbook
workbook.Save("ColumnPropertyDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
