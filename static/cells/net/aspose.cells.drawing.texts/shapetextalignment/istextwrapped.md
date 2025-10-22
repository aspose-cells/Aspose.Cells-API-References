##ShapeTextAlignment.IsTextWrapped
ShapeTextAlignment property. Gets or sets the text wrapped type of the shape which contains text
## ShapeTextAlignment.IsTextWrapped property
Gets or sets the text wrapped type of the shape which contains text.
```csharp
public bool IsTextWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyIsTextWrappedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
// Set shape text
shape.Text = "This is a long text that should be wrapped when IsTextWrapped is set to true";
// Get text alignment and set IsTextWrapped
ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
shapeTextAlignment.IsTextWrapped = true;
// Save the workbook
workbook.Save("ShapeTextWrappingDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
