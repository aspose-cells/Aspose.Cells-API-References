##ShapeTextAlignment.RightMarginPt
ShapeTextAlignment property. Returns the right margin in unit of Points
## ShapeTextAlignment.RightMarginPt property
Returns the right margin in unit of Points
```csharp
public double RightMarginPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyRightMarginPtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
// Access the text alignment
ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
// Set the right margin in points
shapeTextAlignment.RightMarginPt = 2.0d;
// Verify the property by getting the value back
Console.WriteLine("Right Margin in Points: " + shapeTextAlignment.RightMarginPt);
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
