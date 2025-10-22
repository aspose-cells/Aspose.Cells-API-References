##Shape.Fill
Shape property. Returns a FillFormat object that contains fill formatting properties for the specified shape
## Shape.Fill property
Returns a [`FillFormat`](../fillformat/) object that contains fill formatting properties for the specified shape.
```csharp
public FillFormat Fill { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyFillDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
// Get the fill format of the shape
FillFormat fillFmt = shape.Fill;
// Set solid fill with color
fillFmt.SolidFill.Color = System.Drawing.Color.Red;
// Set transparency
fillFmt.Transparency = 0.5;
// Save the workbook
workbook.Save("ShapeFillDemo.xlsx");
}
}
}
```
### See Also
* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
