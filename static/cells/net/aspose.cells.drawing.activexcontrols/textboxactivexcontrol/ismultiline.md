##TextBoxActiveXControl.IsMultiLine
TextBoxActiveXControl property. Indicates whether the control can display more than one line of text
## TextBoxActiveXControl.IsMultiLine property
Indicates whether the control can display more than one line of text.
```csharp
public bool IsMultiLine { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyIsMultiLineDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
1, 1, 200, 100, 0, 0);
Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox =
(Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Demonstrate IsMultiLine property
if (!textBox.IsMultiLine)
{
textBox.IsMultiLine = true;
textBox.Text = "This is a multi-line text box.\nSecond line of text.";
}
// Save the workbook
workbook.Save("TextBoxActiveXControlIsMultiLineDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
