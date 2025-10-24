##Style.BackgroundThemeColor
Style property. Gets and sets the background theme color
## Style.BackgroundThemeColor property
Gets and sets the background theme color.
```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```
### Remarks
If the background color is not a theme color, NULL will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StylePropertyBackgroundThemeColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a style and set background theme color
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
style.BackgroundThemeColor = themeColor;
// Apply the style to a cell
cells["A1"].SetStyle(style);
// Verify the background theme color
ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
}
}
}
```
### See Also
* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
