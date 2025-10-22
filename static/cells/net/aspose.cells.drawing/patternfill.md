##Class PatternFill
Aspose.Cells.Drawing.PatternFill class. Encapsulates the object that represents pattern fill format
## PatternFill class
Encapsulates the object that represents pattern fill format
```csharp
public class PatternFill : Fill
```
## Properties
| Name | Description |
| --- | --- |
| [BackgroundCellsColor](../../aspose.cells.drawing/patternfill/backgroundcellscolor/) { get; set; } | Gets and sets the foreground [`CellsColor`](../../aspose.cells/cellscolor/) object. |
| [BackgroundColor](../../aspose.cells.drawing/patternfill/backgroundcolor/) { get; set; } | Gets or sets the background Color of the [`Area`](../area/). |
| [BackTransparency](../../aspose.cells.drawing/patternfill/backtransparency/) { get; set; } | Gets or sets the transparency of background color. |
| [ForegroundCellsColor](../../aspose.cells.drawing/patternfill/foregroundcellscolor/) { get; set; } | Gets and sets the foreground [`CellsColor`](../../aspose.cells/cellscolor/) object. |
| [ForegroundColor](../../aspose.cells.drawing/patternfill/foregroundcolor/) { get; set; } | Gets or sets the foreground Color. |
| [ForeTransparency](../../aspose.cells.drawing/patternfill/foretransparency/) { get; set; } | Gets or sets the transparency of foreground color. |
| [Pattern](../../aspose.cells.drawing/patternfill/pattern/) { get; set; } | Gets or sets the fill pattern type |
## Methods
| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Inherited from [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Gets the hash code.(Inherited from [`Fill`](../fill/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
public class DrawingClassPatternFillDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create style for the cell using BackgroundType pattern
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.DiagonalStripe;
style.ForegroundColor = Color.LightBlue;
style.BackgroundColor = Color.DarkBlue;
worksheet.Cells["B2"].SetStyle(style);
worksheet.Cells["B2"].PutValue("PatternFill Demo");
// Create shape and configure its pattern fill
Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 100);
shape.Fill.FillType = FillType.Pattern;
PatternFill shapePatternFill = shape.Fill.PatternFill;
shapePatternFill.Pattern = FillPattern.DiagonalBrick;
shapePatternFill.ForegroundColor = Color.LightBlue;
shapePatternFill.BackgroundColor = Color.DarkBlue;
shapePatternFill.ForeTransparency = 0.2;
shapePatternFill.BackTransparency = 0.3;
CellsColor cellsColor = workbook.CreateCellsColor();
cellsColor.Color = Color.Gold;
shapePatternFill.ForegroundCellsColor = cellsColor;
workbook.Save("PatternFillDemo.xlsx");
}
}
}
```
### See Also
* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
