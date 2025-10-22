##Font.ThemeColor
Font property. Gets and sets the theme color
## Font.ThemeColor property
Gets and sets the theme color.
```csharp
public ThemeColor ThemeColor { get; set; }
```
### Remarks
If the font color is not a theme color, NULL will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyThemeColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set text
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Theme Color Demo");
// Get the style and font
Style style = cell.GetStyle();
Font font = style.Font;
// Create and set theme color
font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
// Apply the style to the cell
cell.SetStyle(style);
// Save the workbook
workbook.Save("ThemeColorDemo.xlsx");
// Verify the theme color
Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
}
}
}
```
### See Also
* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
