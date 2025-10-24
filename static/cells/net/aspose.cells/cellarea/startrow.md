##CellArea.StartRow
CellArea field. Gets or set the start row of this area
## CellArea.StartRow field
Gets or set the start row of this area.
```csharp
public int StartRow;
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellAreaFieldStartRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two CellArea objects
CellArea area1 = new CellArea();
area1.StartRow = 2;
area1.StartColumn = 1;
area1.EndRow = 5;
area1.EndColumn = 3;
CellArea area2 = new CellArea();
area2.StartRow = area1.StartRow; // Demonstrating StartRow usage
area2.StartColumn = area1.StartColumn;
area2.EndRow = area1.EndRow;
area2.EndColumn = area1.EndColumn;
// Verify the areas match
if (area1.StartRow == area2.StartRow &&
area1.StartColumn == area2.StartColumn &&
area1.EndRow == area2.EndRow &&
area1.EndColumn == area2.EndColumn)
{
Console.WriteLine("CellArea objects match successfully");
Console.WriteLine($"StartRow: {area1.StartRow}");
}
else
{
Console.WriteLine("CellArea objects do not match");
}
}
}
}
```
### See Also
* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
