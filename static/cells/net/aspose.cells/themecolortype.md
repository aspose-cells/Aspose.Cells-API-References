##Enum ThemeColorType
Aspose.Cells.ThemeColorType enum. Enumerates the theme color types
## ThemeColorType enumeration
Enumerates the theme color types.
```csharp
public enum ThemeColorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Background1 | `0` |  |
| Text1 | `1` |  |
| Background2 | `2` |  |
| Text2 | `3` |  |
| Accent1 | `4` |  |
| Accent2 | `5` |  |
| Accent3 | `6` |  |
| Accent4 | `7` |  |
| Accent5 | `8` |  |
| Accent6 | `9` |  |
| Hyperlink | `10` |  |
| FollowedHyperlink | `11` |  |
| StyleColor | `12` | Inner used. A color used in theme definitions which means to use the color of the style. |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellsClassThemeColorTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Access cell A1 and get its style
Style style = cells["A1"].GetStyle();
// Set solid pattern with red foreground color
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = Color.Red;
Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
// Set gray12 pattern with blue foreground and yellow background
style.Pattern = BackgroundType.Gray12;
style.ForegroundColor = Color.Blue;
style.BackgroundColor = Color.Yellow;
Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
Console.WriteLine("Background ARGB Color: " + style.BackgroundArgbColor);
// Set theme colors
ThemeColor foregroundTheme = new ThemeColor(ThemeColorType.Accent6, 0.5);
ThemeColor backgroundTheme = new ThemeColor(ThemeColorType.Accent2, 0.5);
style.ForegroundThemeColor = foregroundTheme;
style.BackgroundThemeColor = backgroundTheme;
Console.WriteLine("Foreground Theme Color Type: " + style.ForegroundThemeColor.ColorType);
Console.WriteLine("Background Theme Color Type: " + style.BackgroundThemeColor.ColorType);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
