##Cells.MinRow
Cells property. Minimum row index of cell which contains data or style
## Cells.MinRow property
Minimum row index of cell which contains data or style.
```csharp
public int MinRow { get; }
```
### Remarks
This property needs to iterate and check cells and rows dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyMinRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add some data to demonstrate MinRow
cells["A1"].PutValue("Data in first row");
cells["B5"].PutValue("Data in fifth row");
// Display MinRow information
Console.WriteLine("Minimum used row: " + cells.MinRow);
Console.WriteLine("Maximum used row: " + cells.MaxRow);
// Clear contents starting from MinRow
cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);
// Verify clearing by checking if cells are empty
Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
