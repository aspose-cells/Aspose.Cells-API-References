##UnionRange.UnMerge
UnionRange method. Unmerges merged cells of this range
## UnionRange.UnMerge method
Unmerges merged cells of this range.
```csharp
public void UnMerge()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodUnMergeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range and merge cells
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
// Merge the cells and put a value
unionRange.Merge();
unionRange.PutValue("Merged Cells", true, true);
try
{
// Call the UnMerge method
unionRange.UnMerge();
Console.WriteLine("Cells unmerged successfully");
// Put values in the unmerged cells to demonstrate the effect
worksheet.Cells["A1"].PutValue("A1");
worksheet.Cells["A2"].PutValue("A2");
worksheet.Cells["B1"].PutValue("B1");
worksheet.Cells["B2"].PutValue("B2");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
}
// Save the result
workbook.Save("MethodUnMergeDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
