##TextBoxActiveXControl.BorderStyle
TextBoxActiveXControl property. Gets and set the type of border used by the control
## TextBoxActiveXControl.BorderStyle property
Gets and set the type of border used by the control.
```csharp
public ControlBorderType BorderStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyBorderStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an ActiveX TextBox control
var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 100, 100, 0);
TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
// Set the BorderStyle property
textBox.BorderStyle = ControlBorderType.Single;
// Save the workbook
workbook.Save("TextBoxActiveXControlBorderStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlBorderType](../../controlbordertype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
