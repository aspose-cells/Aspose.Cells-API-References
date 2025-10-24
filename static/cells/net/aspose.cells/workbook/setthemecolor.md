##Workbook.SetThemeColor
Workbook method. Sets the theme color
## Workbook.SetThemeColor method
Sets the theme color
```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ThemeColorType | The theme color type. |
| color | Color | the theme color |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodSetThemeColorWithThemeColorTypeColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set theme color for Text1 to Green
workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
// Apply the theme color to default style
Style style = workbook.DefaultStyle;
style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
workbook.DefaultStyle = style;
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("Workbook with theme color saved successfully.");
}
}
}
```
### See Also
* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
