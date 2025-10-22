##Shape.TextDirection
Shape property. Gets/Sets the direction of the text flow for this object
## Shape.TextDirection property
Gets/Sets the direction of the text flow for this object.
```csharp
public TextDirectionType TextDirection { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextDirectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
shape.Text = "Sample Text";
// Set and demonstrate TextDirection property
shape.TextDirection = TextDirectionType.Context;
Console.WriteLine("Initial TextDirection: " + shape.TextDirection);
// Change text direction
shape.TextDirection = TextDirectionType.LeftToRight;
Console.WriteLine("Updated TextDirection: " + shape.TextDirection);
// Save the workbook
workbook.Save("TextDirectionDemo.xlsx");
}
}
}
```
### See Also
* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
