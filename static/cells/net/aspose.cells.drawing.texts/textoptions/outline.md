##TextOptions.Outline
TextOptions property. Represents the outline format of the text
## TextOptions.Outline property
Represents the outline format of the text.
```csharp
public LineFormat Outline { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextOptionsPropertyOutlineDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with text
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
shape.Text = "Sample Text";
// Access text options
TextOptions textOptions = shape.TextOptions;
// Configure outline properties
LineFormat outline = textOptions.Outline;
outline.Weight = 2.48; // Set outline weight
outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
outline.CompoundType = MsoLineStyle.Single; // Set compound type
// Save the workbook
workbook.Save("TextOutlineDemo.xlsx");
}
}
}
```
### See Also
* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
