##Enum BorderType
Aspose.Cells.BorderType enum. Enumerates the border line and diagonal line types
## BorderType enumeration
Enumerates the border line and diagonal line types.
```csharp
[Flags]
public enum BorderType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| LeftBorder | `1` | Represents left border line. |
| RightBorder | `2` | Represents right border line exists. |
| TopBorder | `4` | Represents top border line. |
| BottomBorder | `8` | Represents bottom border line. |
| DiagonalDown | `10` | Represents the diagonal line from top left to right bottom. |
| DiagonalUp | `20` | Represents the diagonal line from bottom left to right top. |
| Vertical | `40` | Only for dynamic style, such as conditional formatting. |
| Horizontal | `80` | Only for dynamic style, such as conditional formatting. |
| SideBorders | `F` | Indicates the four side borders: LeftBorder, RightBorder, TopBorder and BottomBorder. |
| Diagonal | `30` | Special combination of multiple borders for user's convenience for some APIs. Indicates diagonal borders of DiagonalUp and DiagonalDown. |
| DynamicStyleBorders | `C0` | Indicates Vertical and Horizontal of dynamic style. |
| None | `0` | No border has been specified. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class BorderTypeDemo
{
public static void BorderTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a range of cells
var range = worksheet.Cells.CreateRange("A1:D4");
// Create a style object
Style style = workbook.CreateStyle();
// Set the borders for the range
style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);
// Apply the style to the range
StyleFlag flag = new StyleFlag { Borders = true };
range.ApplyStyle(style, flag);
// Save the workbook
workbook.Save("BorderTypeExample.xlsx");
workbook.Save("BorderTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
