##Shape.TextVerticalAlignment
Shape property. Gets and sets the text vertical alignment type of the shape
## Shape.TextVerticalAlignment property
Gets and sets the text vertical alignment type of the shape.
```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextVerticalAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
// Set text and alignment
shape.Text = "Vertical Alignment Demo";
shape.TextVerticalAlignment = TextAlignmentType.Bottom;
Console.WriteLine("Initial Vertical Alignment: " + shape.TextVerticalAlignment);
// Change vertical alignment
if (shape.TextVerticalAlignment == TextAlignmentType.Bottom)
{
shape.TextVerticalAlignment = TextAlignmentType.Center;
}
Console.WriteLine("Updated Vertical Alignment: " + shape.TextVerticalAlignment);
// Save the workbook
workbook.Save("TextVerticalAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
