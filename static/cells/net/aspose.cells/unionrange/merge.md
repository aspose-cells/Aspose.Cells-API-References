##UnionRange.Merge
UnionRange method. Combines a range of cells into a single cell
## UnionRange.Merge method
Combines a range of cells into a single cell.
```csharp
public void Merge()
```
### Remarks
Reference the merged cell via the address of the upper-left cell in the range.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodMergeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range of cells (A1:B2)
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
// Put some data in the cells to visualize merging
range[0, 0].PutValue("Before Merge");
range[0, 1].PutValue("A1");
range[1, 0].PutValue("B1");
range[1, 1].PutValue("B2");
try
{
// Create a UnionRange from the Range
UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
// Call the Merge method
unionRange.Merge();
// Put value in the merged cell
unionRange.PutValue("Merged A1:B2", true, true);
Console.WriteLine("Cells merged successfully");
// Uncomment to see the effect of unmerging
// unionRange.UnMerge();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Merge method: {ex.Message}");
}
// Save the result
workbook.Save("MethodMergeDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
