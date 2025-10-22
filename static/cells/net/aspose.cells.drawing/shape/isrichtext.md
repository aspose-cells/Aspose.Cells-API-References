##Shape.IsRichText
Shape property. Whether or not the text is rich text
## Shape.IsRichText property
Whether or not the text is rich text.
```csharp
public bool IsRichText { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsRichTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with text
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
shape.Text = "This is <b>rich</b> text";
// Check if the text is rich text
if (shape.IsRichText)
{
Console.WriteLine("The text is rich text.");
}
else
{
Console.WriteLine("The text is not rich text.");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
