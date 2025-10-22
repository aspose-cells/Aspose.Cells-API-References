##UnionRange.CellCount
UnionRange property. Gets all cell count in the range
## UnionRange.CellCount property
Gets all cell count in the range.
```csharp
public int CellCount { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangePropertyCellCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate data in the worksheet
for (int row = 0; row < 5; row++)
{
for (int col = 0; col < 5; col++)
{
worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
}
}
// Create ranges and combine them into a union range
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B3");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("D1:E4");
UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });
// Display CellCount property
Console.WriteLine("Total cells in union range: " + unionRange.CellCount);
// Calculate expected cell count
int expectedCount = (range1.RowCount * range1.ColumnCount) + (range2.RowCount * range2.ColumnCount);
Console.WriteLine("Expected cell count: " + expectedCount);
// Demonstrate usage by iterating through cells
Console.WriteLine("\nCell values in the union range:");
int cellCounter = 0;
foreach (Cell cell in unionRange)
{
Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
cellCounter++;
}
// Verify the cell count matches the iteration
Console.WriteLine($"\nIterated through {cellCounter} cells (should match CellCount)");
// Create another union range with different dimensions
Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A5:E5");
Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("C1:C5");
UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });
// Compare cell counts of different union ranges
Console.WriteLine("\nSecond union range cell count: " + unionRange2.CellCount);
Console.WriteLine("First union range has " +
(unionRange.CellCount > unionRange2.CellCount ? "more" : "fewer") +
" cells than second union range");
// Save the workbook
workbook.Save("UnionRangeCellCountDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
