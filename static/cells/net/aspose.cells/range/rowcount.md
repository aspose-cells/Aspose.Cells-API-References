##Range.RowCount
Range property. Gets the count of rows in the range
## Range.RowCount property
Gets the count of rows in the range.
```csharp
public int RowCount { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyRowCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data in cells A1:B10
for (int row = 0; row < 10; row++)
{
for (int col = 0; col < 2; col++)
{
worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
}
}
// Create a named range covering A1:B10
worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
// Get the named range
Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
// Demonstrate RowCount property
Console.WriteLine($"Range starts at row: {range.FirstRow}");
Console.WriteLine($"Range row count: {range.RowCount}");
Console.WriteLine($"Range starts at column: {range.FirstColumn}");
Console.WriteLine($"Range column count: {range.ColumnCount}");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
