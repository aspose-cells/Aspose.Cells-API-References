##ThemeColor.ColorType
ThemeColor property. Gets and sets the theme type
## ThemeColor.ColorType property
Gets and sets the theme type.
```csharp
public ThemeColorType ColorType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThemeColorPropertyColorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create two theme colors with different types
ThemeColor color1 = new ThemeColor(ThemeColorType.Accent1, 0.5);
ThemeColor color2 = new ThemeColor(ThemeColorType.Accent2, 0.3);
// Demonstrate ColorType property
Console.WriteLine("Color1 Type: " + color1.ColorType);
Console.WriteLine("Color2 Type: " + color2.ColorType);
// Apply theme colors to cells
Style style1 = workbook.CreateStyle();
style1.ForegroundThemeColor = color1;
worksheet.Cells["A1"].SetStyle(style1);
Style style2 = workbook.CreateStyle();
style2.ForegroundThemeColor = color2;
worksheet.Cells["A2"].SetStyle(style2);
// Save the workbook
workbook.Save("ThemeColorDemo.xlsx");
}
}
}
```
### See Also
* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
