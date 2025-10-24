##Shape.TextHorizontalOverflow
Shape property. Gets and sets the text horizontal overflow type of the shape which contains text
## Shape.TextHorizontalOverflow property
Gets and sets the text horizontal overflow type of the shape which contains text.
```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextHorizontalOverflowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape with correct parameters
TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
textBox.Text = "This is a long text that will demonstrate text horizontal overflow functionality";
// Set initial overflow type to Clip
textBox.TextHorizontalOverflow = TextOverflowType.Clip;
Console.WriteLine("TextHorizontalOverflow set to Clip (text will be clipped)");
// Change overflow type to Overflow
textBox.TextHorizontalOverflow = TextOverflowType.Overflow;
Console.WriteLine("TextHorizontalOverflow changed to Overflow (text will overflow)");
// Save the workbook
workbook.Save("TextHorizontalOverflowDemo.xlsx");
}
}
}
```
### See Also
* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
