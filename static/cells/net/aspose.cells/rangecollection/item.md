##RangeCollection.Item
RangeCollection property. Gets the Range element at the specified index
## RangeCollection indexer
Gets the [`Range`](../../range/) element at the specified index.
```csharp
public Range this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create some ranges
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");
// Add ranges to the collection
RangeCollection ranges = worksheet.Cells.Ranges;
ranges.Add(range1);
ranges.Add(range2);
ranges.Add(range3);
// Demonstrate Item property usage
Console.WriteLine("Range Collection Count: " + ranges.Count);
for (int i = 0; i < ranges.Count; i++)
{
Aspose.Cells.Range currentRange = ranges[i]; // Using Item property
Console.WriteLine($"Range {i + 1}: {currentRange.Address}");
Console.WriteLine($"  - FirstRow: {currentRange.FirstRow}");
Console.WriteLine($"  - FirstColumn: {currentRange.FirstColumn}");
Console.WriteLine($"  - RowCount: {currentRange.RowCount}");
Console.WriteLine($"  - ColumnCount: {currentRange.ColumnCount}");
}
// Access specific range by index
Aspose.Cells.Range secondRange = ranges[1]; // Using Item property
Console.WriteLine("\nSecond range details:");
Console.WriteLine($"Address: {secondRange.Address}");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
