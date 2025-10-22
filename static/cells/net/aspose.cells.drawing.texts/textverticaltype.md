##Enum TextVerticalType
Aspose.Cells.Drawing.Texts.TextVerticalType enum. Represents the text direct type
## TextVerticalType enumeration
Represents the text direct type.
```csharp
public enum TextVerticalType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Vertical | `0` | East Asian Vertical display. |
| Horizontal | `1` | Horizontal text. |
| VerticalLeftToRight | `2` | Displayed vertical and the text flows top down then LEFT to RIGHT |
| Vertical90 | `3` | Each line is 90 degrees rotated clockwise |
| Vertical270 | `4` | Each line is 270 degrees rotated clockwise |
| Stacked | `5` | Determines if all of the text is vertical |
| StackedRightToLeft | `6` | Specifies that vertical WordArt should be shown from right to left rather than left to right. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextVerticalTypeDemo
{
public static void TextVerticalTypeExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adding a rectangle shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
// Accessing the text alignment settings of the shape
ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
// Setting the text vertical type to Horizontal
shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;
// Setting other properties for demonstration
shapeTextAlignment.IsTextWrapped = true;
shapeTextAlignment.RotateTextWithShape = true;
shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
shapeTextAlignment.RotationAngle = 90;
shapeTextAlignment.IsLockedText = false;
shapeTextAlignment.AutoSize = false;
shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;
shapeTextAlignment.TopMarginPt = 2.0d;
shapeTextAlignment.BottomMarginPt = 2.0d;
shapeTextAlignment.LeftMarginPt = 2.0d;
shapeTextAlignment.RightMarginPt = 2.0d;
shapeTextAlignment.IsAutoMargin = true;
shapeTextAlignment.NumberOfColumns = 1;
// Saving the workbook
workbook.Save("TextVerticalTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
