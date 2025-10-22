##Range.SetStyle
Range method. Apply the cell style
## SetStyle(Style, bool) {#setstyle_1}
Apply the cell style.
```csharp
public void SetStyle(Style style, bool explicitFlag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | Boolean | True, only overwriting formatting which is explicitly set. |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RangeMethodSetStyleWithStyleBooleanDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Style style = wb.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = Color.Red;
Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(0, 0, 1, 5);
range.SetStyle(style, true);
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetStyle(Style) {#setstyle}
Sets the style of the range.
```csharp
public void SetStyle(Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The Style object. |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RangeMethodSetStyleWithStyleDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
style.Font.IsBold = true;
style.Font.Color = Color.Red;
style.Font.Underline = FontUnderlineType.Single;
// Apply the style to a cell
worksheet.Cells["A1"].PutValue("Sample Text");
worksheet.Cells["A1"].SetStyle(style);
// Create a range and apply the same style
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "C3");
range.SetStyle(style);
// Save the workbook
workbook.Save("RangeMethodSetStyleWithStyleDemo_output.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
