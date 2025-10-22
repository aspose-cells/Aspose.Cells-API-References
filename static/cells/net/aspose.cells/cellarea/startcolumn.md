##CellArea.StartColumn
CellArea field. Gets or set the start column of this area
## CellArea.StartColumn field
Gets or set the start column of this area.
```csharp
public int StartColumn;
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellAreaFieldStartColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set some initial data
cells["A1"].PutValue("Header");
cells["A2"].PutValue(10);
cells["A3"].PutValue(20);
// Create a CellArea and set its StartColumn
CellArea area = new CellArea();
area.StartRow = 1;
area.EndRow = 3;
area.StartColumn = 0; // Using StartColumn field
area.EndColumn = 0;
// Insert a new column by shifting existing cells down
cells.InsertRange(area, ShiftType.Down);
// Verify the result
Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
}
}
}
```
### See Also
* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
