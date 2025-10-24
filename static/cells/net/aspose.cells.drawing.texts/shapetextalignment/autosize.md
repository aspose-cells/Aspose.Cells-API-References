##ShapeTextAlignment.AutoSize
ShapeTextAlignment property. Indicates if size of shape is adjusted automatically according to its content
## ShapeTextAlignment.AutoSize property
Indicates if size of shape is adjusted automatically according to its content.
```csharp
public bool AutoSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyAutoSizeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
textBox.Text = "This is a sample text that will demonstrate AutoSize property functionality";
// Get text alignment
ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;
// Demonstrate AutoSize = false (default)
shapeTextAlignment.AutoSize = false;
Console.WriteLine("AutoSize false - Fixed size: " + textBox.Width + "x" + textBox.Height);
// Demonstrate AutoSize = true
shapeTextAlignment.AutoSize = true;
Console.WriteLine("AutoSize true - Auto sized: " + textBox.Width + "x" + textBox.Height);
// Save the workbook
workbook.Save("ShapeTextAlignmentAutoSizeDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
