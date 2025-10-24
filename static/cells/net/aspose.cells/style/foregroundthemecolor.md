##Style.ForegroundThemeColor
Style property. Gets and sets the foreground theme color
## Style.ForegroundThemeColor property
Gets and sets the foreground theme color.
```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```
### Remarks
If the foreground color is not a theme color, NULL will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyForegroundThemeColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Foreground Theme Color Demo");
Style style = cells["A1"].GetStyle();
style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Accent1, -0.25);
style.Pattern = BackgroundType.Solid;
cells["A1"].SetStyle(style);
workbook.Save("ForegroundThemeColorDemo.xlsx");
}
}
}
```
### See Also
* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
