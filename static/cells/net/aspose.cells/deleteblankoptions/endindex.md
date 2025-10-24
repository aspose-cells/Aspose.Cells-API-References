##DeleteBlankOptions.EndIndex
DeleteBlankOptions property. Specifies the end row/column indexinclusive of the range to check and delete blank rows/columns. Default value is 1 and 1 means the maximum range of all objectscells drawings ... that need to be checked
## DeleteBlankOptions.EndIndex property
Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.
```csharp
public int EndIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DeleteBlankOptionsPropertyEndIndexDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Populate some cells with values
cells[0, 2].PutValue(2);
cells[0, 5].PutValue(5);
cells[0, 9].PutValue(9);
// Create delete options with specific range
DeleteBlankOptions dbo = new DeleteBlankOptions();
dbo.StartIndex = 4;
dbo.EndIndex = 7;
// Delete blank columns within specified range
cells.DeleteBlankColumns(dbo);
// Output results to demonstrate the effect of EndIndex
Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
}
}
}
```
### See Also
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
