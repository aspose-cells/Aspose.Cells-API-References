##ColorHelper.FromOleColor
ColorHelper method. Convert OLE_COLOR
## ColorHelper.FromOleColor method
Convert OLE_COLOR.
```csharp
public static Color FromOleColor(int oleColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| oleColor | Int32 | The value of OLE_COLOR. |
### Return Value
The Color object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class ColorHelperMethodFromOleColorWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int oleColor = 0x00FF0000; // OLE color for blue in BGR format
try
{
Color convertedColor = ColorHelper.FromOleColor(oleColor);
// Apply color to cell background
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Color converted from OLE");
Style style = cell.GetStyle();
style.ForegroundColor = convertedColor;
style.Pattern = BackgroundType.Solid;
cell.SetStyle(style);
Console.WriteLine($"Converted OLE color {oleColor:X} to RGB: {convertedColor.Name}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("ColorHelperMethodFromOleColorWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [ColorHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
