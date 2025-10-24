##DeleteBlankOptions.MergedCellsShrinkType
DeleteBlankOptions property. Indicates how to process merged cells when deleting blank rows/columns
## DeleteBlankOptions.MergedCellsShrinkType property
Indicates how to process merged cells when deleting blank rows/columns.
```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```
### Remarks
For KeepHeaderOnly, all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property. For None, all cells in it will be taken as non-blank. For ShrinkToFit, all cells outside the content display area will be taken as blank.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DeleteBlankOptionsPropertyMergedCellsShrinkTypeDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
Cells cells = ws.Cells;
// Setup sample data with merged cells
cells.Merge(0, 0, 3, 1);
cells[0, 0].PutValue("Merged Header");
cells[3, 0].PutValue("Data after blank");
// Create delete options with different shrink types
DeleteBlankOptions options = new DeleteBlankOptions();
// Case 1: KeepHeaderOnly
options.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
cells.DeleteBlankRows(options);
Console.WriteLine("After KeepHeaderOnly - Merged area preserved: " +
(cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
// Reset worksheet
cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
cells.UnMerge(0, 0, 3, 1);
cells.Merge(0, 0, 3, 1);
cells[0, 0].PutValue("Merged Header");
cells[3, 0].PutValue("Data after blank");
// Case 2: ShrinkToFit
options.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
cells.DeleteBlankRows(options);
Console.WriteLine("After ShrinkToFit - Merged area adjusted: " +
(cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
// Reset worksheet
cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
cells.UnMerge(0, 0, 3, 1);
cells.Merge(0, 0, 3, 1);
cells[0, 0].PutValue("Merged Header");
cells[3, 0].PutValue("Data after blank");
// Case 3: None
options.MergedCellsShrinkType = MergedCellsShrinkType.None;
cells.DeleteBlankRows(options);
Console.WriteLine("After None - Merged area unchanged: " +
(cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
}
}
}
```
### See Also
* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
