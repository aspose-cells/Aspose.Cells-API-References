##TextBoxActiveXControl.IsWordWrapped
TextBoxActiveXControl property. Indicates whether the contents of the control automatically wrap at the end of a line
## TextBoxActiveXControl.IsWordWrapped property
Indicates whether the contents of the control automatically wrap at the end of a line.
```csharp
public bool IsWordWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyIsWordWrappedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
1, 1, 200, 100, 0, 0);
Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox =
(Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Set some text that would benefit from word wrapping
textBox.Text = "This is a long text that should demonstrate word wrapping functionality in the TextBox ActiveX control.";
// Check and set IsWordWrapped property
if (!textBox.IsWordWrapped)
{
textBox.IsWordWrapped = true;
Console.WriteLine("Word wrapping has been enabled for the TextBox.");
}
// Save the workbook
workbook.Save("TextBoxWordWrapDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
