##Class Border
Aspose.Cells.Border class. Encapsulates the object that represents the cell border
## Border class
Encapsulates the object that represents the cell border.
```csharp
public class Border
```
## Properties
| Name | Description |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | Gets and sets the color with a 32-bit ARGB value. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Gets or sets the Color of the border. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Gets or sets the cell border type. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Gets and sets the theme color of the border. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class BorderDemo
{
public static void BorderExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Adding a new worksheet to the Workbook object
workbook.Worksheets.Add();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[0];
// Accessing the "A1" cell from the worksheet
Cell cell = worksheet.Cells["A1"];
// Adding some value to the "A1" cell
cell.PutValue("Hello World");
// Getting the cell style
Style style = cell.GetStyle();
// Setting the line style of the top border
Border topBorder = style.Borders[BorderType.TopBorder];
topBorder.LineStyle = CellBorderType.Medium;
topBorder.Color = Color.Red;
// Setting the line style of the bottom border
Border bottomBorder = style.Borders[BorderType.BottomBorder];
bottomBorder.LineStyle = CellBorderType.Thick;
bottomBorder.Color = Color.Blue;
// Setting the line style of the left border
Border leftBorder = style.Borders[BorderType.LeftBorder];
leftBorder.LineStyle = CellBorderType.Dashed;
leftBorder.Color = Color.Green;
// Setting the line style of the right border
Border rightBorder = style.Borders[BorderType.RightBorder];
rightBorder.LineStyle = CellBorderType.Dotted;
rightBorder.Color = Color.Purple;
// Applying the style to the cell
cell.SetStyle(style);
// Saving the Excel file
workbook.Save("BorderExample.xlsx");
workbook.Save("BorderExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
