##Enum MergedCellsShrinkType
Aspose.Cells.MergedCellsShrinkType enum. Represents the strategy to shrink merged cells for operations such as deleting blank rows/column
## MergedCellsShrinkType enumeration
Represents the strategy to shrink merged cells for operations such as deleting blank rows/column.
```csharp
public enum MergedCellsShrinkType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Leaves the merged cells as it is without any modification. |
| ShrinkToFit | `1` | Shrinks the merged area if needed, by removing rows from the bottom or columns from the right, while ensuring all content remains visible. |
| KeepHeaderOnly | `2` | Only keeps the header rows/columns of the merged area when the top-left cell of the merged area is not blank. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassMergedCellsShrinkTypeDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
Cells cells = ws.Cells;
// Initialize sample data with merged cells
cells.Merge(0, 0, 1, 2);
cells[0, 0].PutValue("Merged Header");
cells[1, 2].PutValue("Data 1");
cells[2, 2].PutValue("Data 2");
Console.WriteLine("Original worksheet:");
PrintCellValues(cells);
// Option 1: KeepHeaderOnly
DeleteBlankOptions opts1 = new DeleteBlankOptions();
opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
cells.DeleteBlankColumns(opts1);
Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
PrintCellValues(cells);
// Reset worksheet
cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
cells.Merge(0, 0, 1, 2);
cells[0, 0].PutValue("Merged Header");
cells[1, 2].PutValue("Data 1");
cells[2, 2].PutValue("Data 2");
// Option 2: None
DeleteBlankOptions opts2 = new DeleteBlankOptions();
opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
cells.DeleteBlankColumns(opts2);
Console.WriteLine("\nAfter DeleteBlankColumns with None:");
PrintCellValues(cells);
// Reset worksheet
cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
cells.Merge(0, 0, 1, 2);
cells[0, 0].PutValue("Merged Header");
cells[1, 2].PutValue("Data 1");
cells[2, 2].PutValue("Data 2");
// Option 3: ShrinkToFit
DeleteBlankOptions opts3 = new DeleteBlankOptions();
opts3.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
cells.DeleteBlankColumns(opts3);
Console.WriteLine("\nAfter DeleteBlankColumns with ShrinkToFit:");
PrintCellValues(cells);
}
private static void PrintCellValues(Cells cells)
{
for (int row = 0; row < 3; row++)
{
for (int col = 0; col < 3; col++)
{
Console.Write($"({row},{col}): {cells[row, col].Value ?? "empty"} | ");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
