##Class ColorHelper
Aspose.Cells.Drawing.ColorHelper class. Provides helper functions about color
## ColorHelper class
Provides helper functions about color.
```csharp
public class ColorHelper
```
## Methods
| Name | Description |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | Convert OLE_COLOR. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | Convert color to OLE_COLOR |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
public class DrawingClassColorHelperDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Convert OLE color to System.Drawing.Color (Green)
int oleGreen = 0x00FF00;
Color colorFromOle = ColorHelper.FromOleColor(oleGreen);
// Apply converted color to cell A1 background
Cell cellA1 = worksheet.Cells["A1"];
Style styleA1 = cellA1.GetStyle();
styleA1.ForegroundColor = colorFromOle;
styleA1.Pattern = BackgroundType.Solid;
cellA1.SetStyle(styleA1);
// Convert System.Drawing.Color back to OLE color
int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);
// Convert OLE result back to Color (verification)
Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);
// Apply re-converted color to cell A2 background
Cell cellA2 = worksheet.Cells["A2"];
Style styleA2 = cellA2.GetStyle();
styleA2.ForegroundColor = colorFromConvertedOle;
styleA2.Pattern = BackgroundType.Solid;
cellA2.SetStyle(styleA2);
// Save the modified workbook
workbook.Save("DrawingClassColorHelperDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
