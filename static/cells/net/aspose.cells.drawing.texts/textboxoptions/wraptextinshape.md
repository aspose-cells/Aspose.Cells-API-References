##TextBoxOptions.WrapTextInShape
TextBoxOptions property. Specifies text wrapping within a shape. False  No wrapping will occur on text body. True  Wrapping will occur on text body
## TextBoxOptions.WrapTextInShape property
Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body.
```csharp
public bool WrapTextInShape { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyWrapTextInShapeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape with correct parameters
TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
// Set text that will wrap within the shape
textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";
// Enable text wrapping within the shape
textBox.TextBoxOptions.WrapTextInShape = true;
// Save the workbook
workbook.Save("TextBoxWrapTextDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
