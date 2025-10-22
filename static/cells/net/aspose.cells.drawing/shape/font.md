##Shape.Font
Shape property. Represents the font of shape
## Shape.Font property
Represents the font of shape.
```csharp
public Font Font { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Access and modify the font properties of the shape
Aspose.Cells.Font font = shape.Font;
font.Name = "Arial";
font.Size = 12;
font.Color = Color.Red;
// Save the workbook
workbook.Save("ShapeFontDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
