##Cell.Copy
Cell method. Copies data from a source cell
## Cell.Copy method
Copies data from a source cell.
```csharp
public void Copy(Cell cell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Source [`Cell`](../) object. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodCopyWithCellDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set values and styles in source cell
Cell sourceCell = cells["A1"];
sourceCell.PutValue("Source Value");
sourceCell.GetStyle().Font.IsBold = true;
// Create destination cell
Cell destCell = cells["B1"];
// Copy from source to destination
destCell.Copy(sourceCell);
// Verify the copy
Console.WriteLine("Destination cell value: " + destCell.StringValue);
Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
