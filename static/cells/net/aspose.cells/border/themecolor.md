##Border.ThemeColor
Border property. Gets and sets the theme color of the border
## Border.ThemeColor property
Gets and sets the theme color of the border.
```csharp
public ThemeColor ThemeColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BorderPropertyThemeColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access a cell and get its style
Style style = worksheet.Cells["A1"].GetStyle();
// Set border theme color
style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
// Apply the style to the cell
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("BorderThemeColorDemo.xlsx");
}
}
}
```
### See Also
* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
