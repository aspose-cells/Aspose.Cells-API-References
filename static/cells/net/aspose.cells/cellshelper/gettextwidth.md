##CellsHelper.GetTextWidth
CellsHelper method. Get width of text in unit of points
## CellsHelper.GetTextWidth method
Get width of text in unit of points.
```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```
| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text. |
| font | Font | The font of the text. |
| scaling | Double | The scaling of text. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Font font = workbook.DefaultStyle.Font;
double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
Console.WriteLine("Text width: " + textWidth);
}
}
}
```
### See Also
* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
