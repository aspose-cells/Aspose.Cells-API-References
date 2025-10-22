##Cell.GetMergedRange
Cell method. Returns a Range object which represents a merged range
## Cell.GetMergedRange method
Returns a [`Range`](../../range/) object which represents a merged range.
```csharp
public Range GetMergedRange()
```
### Return Value
[`Range`](../../range/) object. Null if this cell is not merged.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetMergedRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Merge cells
cells.Merge(0, 0, 2, 2);
// Get the first cell
Cell cell = cells[0, 0];
// Get merged range information
Aspose.Cells.Range mergedRange = cell.GetMergedRange();
// Output merged range details
Console.WriteLine("Merged Range Details:");
Console.WriteLine($"First Row: {mergedRange.FirstRow}");
Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
Console.WriteLine($"Row Count: {mergedRange.RowCount}");
Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
