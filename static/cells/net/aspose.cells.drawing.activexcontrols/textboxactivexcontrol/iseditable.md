##TextBoxActiveXControl.IsEditable
TextBoxActiveXControl property. Indicates whether the user can type into the control
## TextBoxActiveXControl.IsEditable property
Indicates whether the user can type into the control.
```csharp
public bool IsEditable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyIsEditableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
1, 1, 100, 50, 100, 50);
Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox =
(Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Demonstrate IsEditable property
Console.WriteLine("Initial IsEditable: " + textBox.IsEditable);
// Toggle the IsEditable property
textBox.IsEditable = !textBox.IsEditable;
Console.WriteLine("After toggle IsEditable: " + textBox.IsEditable);
// Save the workbook
workbook.Save("TextBoxActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
