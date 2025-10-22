##Class ThemeColor
Aspose.Cells.ThemeColor class. Represents a theme color
## ThemeColor class
Represents a theme color.
```csharp
public class ThemeColor
```
## Constructors
| Name | Description |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |
## Properties
| Name | Description |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Gets and sets the theme type. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Gets and sets the tint value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ThemeColorDemo
{
public static void ThemeColorExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Adding a value to cell A1
cells["A1"].PutValue("Hello World");
// Getting the style of cell A1
Style style = cells["A1"].GetStyle();
// Set ThemeColorType.Text2 color type with 40% lighten as the font color.
style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
style.Pattern = BackgroundType.Solid;
// Set ThemeColorType.Background2 color type with 75% darken as the foreground color
style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);
// Applying the style to cell A1
cells["A1"].SetStyle(style);
// Saving the Excel file
workbook.Save("ThemeColorExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
