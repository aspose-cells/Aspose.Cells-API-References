##Workbook.GetThemeColor
Workbook method. Gets theme color
## Workbook.GetThemeColor method
Gets theme color.
```csharp
public Color GetThemeColor(ThemeColorType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ThemeColorType | The theme color type. |
### Return Value
The theme color.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodGetThemeColorWithThemeColorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get theme color for Accent6
Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
Console.WriteLine("Theme Color (Accent6): " + color.ToString());
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
