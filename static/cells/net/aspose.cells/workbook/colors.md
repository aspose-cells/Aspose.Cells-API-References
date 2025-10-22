##Workbook.Colors
Workbook property. Returns colors in the palette for the spreadsheet
## Workbook.Colors property
Returns colors in the palette for the spreadsheet.
```csharp
public Color[] Colors { get; }
```
### Remarks
The palette has 56 entries, each represented by an RGB value.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class WorkbookPropertyColorsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the default colors palette
Color[] colors = workbook.Colors;
// Modify some colors in the palette
colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue
// Create a worksheet and add some data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Color Demo");
// Apply the modified colors to cells
Style style1 = workbook.CreateStyle();
style1.ForegroundColor = colors[0];
style1.Pattern = BackgroundType.Solid;
worksheet.Cells["A2"].SetStyle(style1);
Style style2 = workbook.CreateStyle();
style2.ForegroundColor = colors[1];
style2.Pattern = BackgroundType.Solid;
worksheet.Cells["B2"].SetStyle(style2);
Style style3 = workbook.CreateStyle();
style3.ForegroundColor = colors[2];
style3.Pattern = BackgroundType.Solid;
worksheet.Cells["C2"].SetStyle(style3);
// Save the workbook
workbook.Save("WorkbookColorsDemo.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
