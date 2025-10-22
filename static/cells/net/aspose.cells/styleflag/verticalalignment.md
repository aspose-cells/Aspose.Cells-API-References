##StyleFlag.VerticalAlignment
StyleFlag property. Vertical alignment setting will be applied
## StyleFlag.VerticalAlignment property
Vertical alignment setting will be applied.
```csharp
public bool VerticalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyVerticalAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a style with vertical alignment
Style style = workbook.CreateStyle();
style.VerticalAlignment = TextAlignmentType.Center;
style.HorizontalAlignment = TextAlignmentType.Center;
style.Font.Color = Color.Blue;
// Create style flag to only apply vertical alignment and font color
StyleFlag styleFlag = new StyleFlag();
styleFlag.VerticalAlignment = true;
styleFlag.FontColor = true;
// Apply the style to the first row with the style flag
Row row = sheet.Cells.Rows[0];
row.ApplyStyle(style, styleFlag);
// Set some text in the cells to see the effect
sheet.Cells["A1"].PutValue("Vertically Centered");
sheet.Cells["B1"].PutValue("Blue Text");
// Save the workbook
workbook.Save("VerticalAlignmentDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
