##TextBoxActiveXControl.EnterKeyBehavior
TextBoxActiveXControl property. Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that pressing ENTER will move the focus to the next object in the tab order
## TextBoxActiveXControl.EnterKeyBehavior property
Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that pressing ENTER will move the focus to the next object in the tab order.
```csharp
public bool EnterKeyBehavior { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyEnterKeyBehaviorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX Control
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
1, 1, 1, 1, 100, 100);
Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox =
(Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Demonstrate EnterKeyBehavior property
Console.WriteLine("Initial EnterKeyBehavior: " + textBox.EnterKeyBehavior);
// Toggle the EnterKeyBehavior
textBox.EnterKeyBehavior = !textBox.EnterKeyBehavior;
Console.WriteLine("Modified EnterKeyBehavior: " + textBox.EnterKeyBehavior);
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
