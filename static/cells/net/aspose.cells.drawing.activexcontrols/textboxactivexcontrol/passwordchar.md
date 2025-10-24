##TextBoxActiveXControl.PasswordChar
TextBoxActiveXControl property. Gets and sets a character to be displayed in place of the characters entered
## TextBoxActiveXControl.PasswordChar property
Gets and sets a character to be displayed in place of the characters entered.
```csharp
public char PasswordChar { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyPasswordCharDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX Control and get its shape
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 0, 1, 1, 100, 50);
// Get the TextBoxActiveXControl from the shape
Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBoxControl =
(Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Set PasswordChar property
textBoxControl.PasswordChar = '*';
// Set some text to demonstrate the password masking
textBoxControl.Text = "password123";
// Save the workbook
workbook.Save("TextBoxActiveXControlPasswordCharDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
