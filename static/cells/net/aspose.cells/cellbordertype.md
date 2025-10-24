##Enum CellBorderType
Aspose.Cells.CellBorderType enum. Enumerates a cells border type
## CellBorderType enumeration
Enumerates a cell's border type.
```csharp
public enum CellBorderType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DashDot | `9` | Represents thin dash-dotted line. |
| DashDotDot | `11` | Represents thin dash-dot-dotted line. |
| Dashed | `3` | Represents dashed line. |
| Dotted | `4` | Represents dotted line. |
| Double | `6` | Represents double line. |
| Hair | `7` | Represents hair line. |
| MediumDashDot | `10` | Represents medium dash-dotted line. |
| MediumDashDotDot | `12` | Represents medium dash-dot-dotted line. |
| MediumDashed | `8` | Represents medium dashed line. |
| None | `0` | Represents no line. |
| Medium | `2` | Represents medium line. |
| SlantedDashDot | `13` | Represents slanted medium dash-dotted line. |
| Thick | `5` | Represents thick line. |
| Thin | `1` | Represents thin line. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class CellBorderTypeDemo
{
public static void CellBorderTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a range (A1:D4)
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");
// Get the style of the range
Style style = workbook.CreateStyle();
// Set different border styles for the range
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
style.Borders[BorderType.TopBorder].Color = Color.Black;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
style.Borders[BorderType.BottomBorder].Color = Color.Blue;
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
style.Borders[BorderType.LeftBorder].Color = Color.Green;
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
style.Borders[BorderType.RightBorder].Color = Color.Red;
// Apply the style to the range
StyleFlag styleFlag = new StyleFlag();
styleFlag.Borders = true;
range.ApplyStyle(style, styleFlag);
// Save the workbook
workbook.Save("CellBorderTypeExample.xlsx");
workbook.Save("CellBorderTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
