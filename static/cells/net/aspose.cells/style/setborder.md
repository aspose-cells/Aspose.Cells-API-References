##Style.SetBorder
Style method. Sets the borders of the style
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}
Sets the borders of the style.
```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | BorderType | The border(s) to be set, can be combination of [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | The style of the border. |
| borderColor | Color | The color of the border. |
### Return Value
Whether current border settings have been changed.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleMethodSetBorderWithBorderTypeCellBorderTypeColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var range = worksheet.Cells.CreateRange("A1:D4");
Style style = workbook.CreateStyle();
style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);
StyleFlag flag = new StyleFlag { Borders = true };
range.ApplyStyle(style, flag);
workbook.Save("BorderExample.xlsx");
}
}
}
```
### See Also
* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}
Sets the borders of the style.
```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderType | BorderType | The border(s) to be set, can be combination of [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | The style of the border. |
| borderColor | CellsColor | The color of the border. |
### Return Value
Whether current border settings have been changed.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some data for context
worksheet.Cells["A1"].Value = "Border Demo";
try
{
// Create a style
Style style = workbook.CreateStyle();
// Create a CellsColor object using the proper factory method
CellsColor borderColor = workbook.CreateCellsColor();
borderColor.Color = Color.Green;
// Call SetBorder with BorderType, CellBorderType and CellsColor parameters
bool result = style.SetBorder(
BorderType.TopBorder,
CellBorderType.Thick,
borderColor);
// Apply the style to a cell
worksheet.Cells["A1"].SetStyle(style);
Console.WriteLine("SetBorder method called successfully. Result: " + result);
// Save the workbook
workbook.Save("SetBorderDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error calling SetBorder: {ex.Message}");
}
}
}
}
```
### See Also
* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
