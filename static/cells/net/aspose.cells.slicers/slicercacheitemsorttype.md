##Enum SlicerCacheItemSortType
Aspose.Cells.Slicers.SlicerCacheItemSortType enum. Specify the sort type of SlicerCacheItem
## SlicerCacheItemSortType enumeration
Specify the sort type of SlicerCacheItem
```csharp
public enum SlicerCacheItemSortType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Natural | `0` | Original data order. |
| Ascending | `1` | Ascending sort type |
| Descending | `2` | Descending sort type |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Slicers;
using System;
public class SlicersClassSlicerCacheItemSortTypeDemo
{
public static void Run()
{
try
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate all values of SlicerCacheItemSortType enum
Console.WriteLine("Available sort types:");
Console.WriteLine($"Natural: {(int)SlicerCacheItemSortType.Natural}");
Console.WriteLine($"Ascending: {(int)SlicerCacheItemSortType.Ascending}");
Console.WriteLine($"Descending: {(int)SlicerCacheItemSortType.Descending}");
// Show usage in a practical scenario
SlicerCacheItemSortType selectedSortType = SlicerCacheItemSortType.Ascending;
Console.WriteLine($"\nSelected sort type: {selectedSortType} ({(int)selectedSortType})");
// Save the workbook
workbook.Save("SlicerCacheItemSortTypeDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error demonstrating SlicerCacheItemSortType: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)
