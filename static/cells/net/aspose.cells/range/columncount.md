##Range.ColumnCount
Range property. Gets the count of columns in the range
## Range.ColumnCount property
Gets the count of columns in the range.
```csharp
public int ColumnCount { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangePropertyColumnCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Create sample data (5 columns x 3 rows)
for (int col = 0; col < 5; col++)
{
for (int row = 0; row < 3; row++)
{
sheet.Cells[row, col].PutValue($"Data {row},{col}");
}
}
// Create a range covering all data columns
Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
// Demonstrate ColumnCount usage
Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
// Auto-fit each column in the range
for (int i = 0; i < dataRange.ColumnCount; i++)
{
sheet.AutoFitColumn(dataRange.FirstColumn + i);
}
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
