##Enum ShapeAnchorType
Aspose.Cells.Drawing.ShapeAnchorType enum. Represents the anchor type
## ShapeAnchorType enumeration
Represents the anchor type.
```csharp
public enum ShapeAnchorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| TwoCellAnchor | `0` | Represents a two cell anchor placeholder |
| OneCellAnchor | `1` | Represents a one cell anchor placeholder |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassShapeAnchorTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a group box shape
Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
box.Text = "Sample Group Box";
// Demonstrate ShapeAnchorType usage
box.AnchorType = ShapeAnchorType.TwoCellAnchor;
box.UpperLeftRow = 2;
box.UpperLeftColumn = 1;
box.LowerRightRow = 8;
box.LowerRightColumn = 4;
// Save the workbook
workbook.Save("ShapeAnchorTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
