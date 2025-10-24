##Cells.Merge
Cells method. Merges a specified range of cells into a single cell
## Merge(int, int, int, int) {#merge}
Merges a specified range of cells into a single cell.
```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |
### Remarks
Reference the merged cell via the address of the upper-left cell in the range.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodMergeWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Put values in cells to demonstrate merging
cells[0, 0].PutValue("Merged Area");
cells[5, 5].PutValue("Not Merged");
// Merge cells starting from row 0, column 0 spanning 3 rows and 2 columns
cells.Merge(0, 0, 3, 2);
// Save the workbook
workbook.Save("MergeDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Merge(int, int, int, int, bool) {#merge_1}
Merges a specified range of cells into a single cell.
```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns,
bool mergeConflict)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |
| mergeConflict | Boolean | Merge conflict merged ranges. |
### Remarks
Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Merge cells from row 3, column 4 (D3) to row 7, column 5 (E7) - 5 rows and 2 columns
worksheet.Cells.Merge(3, 4, 5, 2, true);
// Save the workbook
workbook.Save("MergeDemoOutput.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Merge(int, int, int, int, bool, bool) {#merge_2}
Merges a specified range of cells into a single cell.
```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns,
bool checkConflict, bool mergeConflict)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |
| checkConflict | Boolean | Indicates whether check the merged cells intersects other merged cells |
| mergeConflict | Boolean | Merge conflict merged ranges. |
### Remarks
Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Put some data in cells to be merged
cells[0, 1].PutValue("Merged Cell");
cells[1, 1].PutValue("This will be merged");
// Merge cells without options (simple merge)
cells.Merge(0, 1, 2, 2);
Console.WriteLine("Cells merged without options");
// Unmerge first to demonstrate next merge
cells.UnMerge(0, 1, 2, 2);
// Merge cells with ignoreStyle=false and mergeConflict=true
cells.Merge(0, 1, 2, 2, false, true);
Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");
// Save the workbook
workbook.Save("MergeCellsDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
