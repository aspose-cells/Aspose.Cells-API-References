##Cells.Ranges
Cells property. Gets the collection of Range objects created at run time
## Cells.Ranges property
Gets the collection of [`Range`](../../range/) objects created at run time.
```csharp
public RangeCollection Ranges { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyRangesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create and add a range to the Ranges collection
Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
worksheet.Cells.Ranges.Add(cellRange);
// Insert rows and demonstrate the range expands
worksheet.Cells.InsertRows(2, 2, true);
Console.WriteLine($"Range row count after insertion: {cellRange.RowCount}");
}
}
}
```
### See Also
* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
