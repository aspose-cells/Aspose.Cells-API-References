##Range.UnMerge
Range method. Unmerges merged cells of this range
## Range.UnMerge method
Unmerges merged cells of this range.
```csharp
public void UnMerge()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodUnMergeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Merge cells B2 to D4
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
range.Merge();
// Check if cell B2 is merged before unmerging
Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
// Unmerge the range
range.UnMerge();
// Check if cell B2 is merged after unmerging
Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
