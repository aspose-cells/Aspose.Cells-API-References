##Cells.MergedCells
Cells property. Gets the collection of merged cells
## Cells.MergedCells property
Gets the collection of merged cells.
```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```
### Remarks
In this collection, each item is a [`CellArea`](../../cellarea/) structure which represents an area of merged cells.
NOTE: This method is now obsolete. Instead, please use Cells.GetMergedAreas() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class CellsPropertyMergedCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Merge cells in two different ranges
cells.Merge(0, 0, 2, 2); // Merges A1:B2
cells.Merge(2, 2, 2, 2); // Merges C3:D4
// Access the MergedCells property (read-only)
ArrayList mergedRanges = cells.MergedCells;
// Display initial merged cells count and ranges
Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
foreach (CellArea area in mergedRanges)
{
Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
}
// Unmerge the first merged range
cells.UnMerge(0, 0, 2, 2);
// Display updated merged cells count and ranges
Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
foreach (CellArea area in cells.MergedCells)
{
Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
}
// Save the result
workbook.Save("PropertyMergedCellsDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
