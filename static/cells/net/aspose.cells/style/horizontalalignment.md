##Style.HorizontalAlignment
Style property. Gets or sets the horizontal alignment type of the text in a cell
## Style.HorizontalAlignment property
Gets or sets the horizontal alignment type of the text in a cell.
```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyHorizontalAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set text in cells
cells["A1"].PutValue("Left Aligned");
cells["A2"].PutValue("Center Aligned");
cells["A3"].PutValue("Right Aligned");
// Get style objects
Style styleLeft = cells["A1"].GetStyle();
Style styleCenter = cells["A2"].GetStyle();
Style styleRight = cells["A3"].GetStyle();
// Set horizontal alignment
styleLeft.HorizontalAlignment = TextAlignmentType.Left;
styleCenter.HorizontalAlignment = TextAlignmentType.Center;
styleRight.HorizontalAlignment = TextAlignmentType.Right;
// Apply styles to cells
cells["A1"].SetStyle(styleLeft);
cells["A2"].SetStyle(styleCenter);
cells["A3"].SetStyle(styleRight);
// Save the workbook
workbook.Save("HorizontalAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
