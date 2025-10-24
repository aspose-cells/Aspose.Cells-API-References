##Range.Merge
Range method. Combines a range of cells into a single cell
## Range.Merge method
Combines a range of cells into a single cell.
```csharp
public void Merge()
```
### Remarks
Reference the merged cell via the address of the upper-left cell in the range.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodMergeDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range and merge cells (3 rows x 2 columns)
Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
range.Merge();
// Set value in the merged cell
worksheet.Cells[0, 0].Value = "Merged Cells Demo";
// Style the merged cells
Style style = worksheet.Cells[0, 0].GetStyle();
style.HorizontalAlignment = TextAlignmentType.Center;
style.VerticalAlignment = TextAlignmentType.Center;
style.Font.IsBold = true;
worksheet.Cells[0, 0].SetStyle(style);
// Save the workbook
workbook.Save("MergedCellsDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
