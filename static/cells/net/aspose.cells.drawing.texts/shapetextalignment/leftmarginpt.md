##ShapeTextAlignment.LeftMarginPt
ShapeTextAlignment property. Returns the left margin in unit of Points
## ShapeTextAlignment.LeftMarginPt property
Returns the left margin in unit of Points
```csharp
public double LeftMarginPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyLeftMarginPtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Set text for the shape
shape.Text = "Sample text with left margin";
// Access text alignment and set left margin in points
ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
textAlignment.LeftMarginPt = 2.0d;
// Save the workbook
workbook.Save("ShapeTextAlignmentLeftMarginPtDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
