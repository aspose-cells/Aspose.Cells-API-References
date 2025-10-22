##Shape.TextOptions
Shape property. Represents the text options of the shape
## Shape.TextOptions property
Represents the text options of the shape.
```csharp
public TextOptions TextOptions { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
// Set text for the shape
shape.Text = "Sample Text";
// Access and modify TextOptions
TextOptions opt = shape.TextOptions;
opt.Color = Color.Blue;
opt.Size = 8;
// Save the workbook
workbook.Save("ShapeTextOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
