##Style.SetPatternColor
Style method. Sets the background color
## Style.SetPatternColor method
Sets the background color.
```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | BackgroundType | The pattern. |
| color1 | Color | The foreground color. |
| color2 | Color | The background color. Only works when pattern is not BackgroundType.None and BackgroundType.Solid. |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleMethodSetPatternColorWithBackgroundTypeColorColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
Style style = cell.GetStyle();
style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Blue);
cell.SetStyle(style);
workbook.Save("SetPatternColorDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
