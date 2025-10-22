##Class ShapeTextAlignment
Aspose.Cells.Drawing.Texts.ShapeTextAlignment class. Represents the setting of shapes text alignment
## ShapeTextAlignment class
Represents the setting of shape's text alignment;
```csharp
public class ShapeTextAlignment
```
## Properties
| Name | Description |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize/) { get; set; } | Indicates if size of shape is adjusted automatically according to its content. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/) { get; set; } | Returns the bottom margin in unit of Points |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin/) { get; set; } | Indicates whether the margin of the text frame is automatic. |
| [IsLockedText](../../aspose.cells.drawing.texts/shapetextalignment/islockedtext/) { get; set; } | Indicates whether the shape is locked when worksheet is protected. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped/) { get; set; } | Gets or sets the text wrapped type of the shape which contains text. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/) { get; set; } | Returns the left margin in unit of Points |
| [NumberOfColumns](../../aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/) { get; set; } | Gets and sets the number of columns of text in the bounding rectangle. |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/) { get; set; } | Returns the right margin in unit of Points |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/) { get; set; } | Indicates whether rotating text with shape. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle/) { get; set; } | Gets and sets the rotation of the shape. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/) { get; set; } | Gets and sets the text horizontal overflow type of the text box. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype/) { get; set; } | Gets and set the transform type of text. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/) { get; set; } | Gets and sets the text vertical overflow type of the text box. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype/) { get; set; } | Gets and sets the text direction. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt/) { get; set; } | Returns the top margin in unit of Points |
## Methods
| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals/)(object) | Determines whether this instance has the same value as another specified `ShapeTextAlignment` object. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode/)() |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class ShapeTextAlignmentDemo
{
public static void ShapeTextAlignmentExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adding a rectangle shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
// Accessing the ShapeTextAlignment object
ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
// Setting properties
shapeTextAlignment.IsTextWrapped = true;
shapeTextAlignment.RotateTextWithShape = true;
shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
shapeTextAlignment.RotationAngle = 90;
shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;
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
workbook.Save("ShapeTextAlignmentExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
