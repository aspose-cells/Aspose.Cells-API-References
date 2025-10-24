##Cells.MaxRow
Cells property. Maximum row index of cell which contains data or style
## Cells.MaxRow property
Maximum row index of cell which contains data or style.
```csharp
public int MaxRow { get; }
```
### Remarks
Return -1 if there is no cell which contains data or style in the worksheet. This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyMaxRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add some sample data
cells[0, 0].PutValue("Name");
cells[0, 1].PutValue("Age");
cells[1, 0].PutValue("John");
cells[1, 1].PutValue(30);
cells[2, 0].PutValue("Alice");
cells[2, 1].PutValue(25);
// Get the max row index (zero-based)
int maxRow = cells.MaxRow;
Console.WriteLine("MaxRow before adding new data: " + maxRow);
// Add new data in the next row after max row
int newRow = maxRow + 1;
cells[newRow, 0].PutValue("Bob");
cells[newRow, 1].PutValue(28);
// Verify the new max row
Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);
// Save the workbook
workbook.Save("MaxRowDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
