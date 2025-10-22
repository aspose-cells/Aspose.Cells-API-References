##TextBoxActiveXControl.EnterFieldBehavior
TextBoxActiveXControl property. Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control
## TextBoxActiveXControl.EnterFieldBehavior property
Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.
```csharp
public bool EnterFieldBehavior { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyEnterFieldBehaviorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX Control with correct parameters
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
1, 1, 1, 1, 100, 50);
Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox =
(Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Demonstrate EnterFieldBehavior property
Console.WriteLine("Initial EnterFieldBehavior: " + textBox.EnterFieldBehavior);
// Toggle the EnterFieldBehavior property
textBox.EnterFieldBehavior = !textBox.EnterFieldBehavior;
Console.WriteLine("Toggled EnterFieldBehavior: " + textBox.EnterFieldBehavior);
// Set EnterFieldBehavior to true explicitly
textBox.EnterFieldBehavior = true;
Console.WriteLine("Final EnterFieldBehavior: " + textBox.EnterFieldBehavior);
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
