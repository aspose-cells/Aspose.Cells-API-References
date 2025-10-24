##Shape.TextHorizontalAlignment
Shape property. Gets and sets the text horizontal alignment type of the shape
## Shape.TextHorizontalAlignment property
Gets and sets the text horizontal alignment type of the shape.
```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextHorizontalAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
// Set text and alignment
shape.Text = "Sample Text";
shape.TextHorizontalAlignment = TextAlignmentType.Center;
// Change alignment if it's currently Bottom
if (shape.TextHorizontalAlignment == TextAlignmentType.Bottom)
{
shape.TextHorizontalAlignment = TextAlignmentType.Center;
}
// Save the workbook
workbook.Save("ShapeTextAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
