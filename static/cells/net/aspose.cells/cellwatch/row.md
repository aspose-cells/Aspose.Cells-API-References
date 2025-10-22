##CellWatch.Row
CellWatch property. Gets and sets the row of the cell
## CellWatch.Row property
Gets and sets the row of the cell.
```csharp
public int Row { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellWatchPropertyRowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to cell B2
sheet.Cells["B2"].PutValue("Sample Data");
// Add CellWatch for B2
int watchIndex = sheet.CellWatches.Add("B2");
CellWatch cellWatch = sheet.CellWatches[watchIndex];
// Demonstrate Row property
Console.WriteLine($"Original Row: {cellWatch.Row}");
cellWatch.Row = 1; // Set row to 1 (0-based) for B2
Console.WriteLine($"Updated Row: {cellWatch.Row}");
// Verify the cell reference
Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");
workbook.Save("CellWatchRowDemo.xlsx");
}
}
}
```
### See Also
* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
