##TextBoxOptions.ResizeToFitText
TextBoxOptions property. Indicates whether to resize the shape to fit the text
## TextBoxOptions.ResizeToFitText property
Indicates whether to resize the shape to fit the text
```csharp
public bool ResizeToFitText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyResizeToFitTextDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a text box with correct parameters
Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
textBox.Text = "This is a sample text that will make the text box resize to fit";
// Access TextBoxOptions correctly
textBox.TextBoxOptions.ResizeToFitText = true;
// Save the workbook
workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
