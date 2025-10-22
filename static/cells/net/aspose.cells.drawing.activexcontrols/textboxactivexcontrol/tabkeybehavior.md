##TextBoxActiveXControl.TabKeyBehavior
TextBoxActiveXControl property. Indicates whether tab characters are allowed in the text of the control
## TextBoxActiveXControl.TabKeyBehavior property
Indicates whether tab characters are allowed in the text of the control.
```csharp
public bool TabKeyBehavior { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyTabKeyBehaviorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX Control and get its ActiveXControl property
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Demonstrate TabKeyBehavior property
Console.WriteLine("Initial TabKeyBehavior: " + textBoxControl.TabKeyBehavior);
// Enable TabKeyBehavior
if (!textBoxControl.TabKeyBehavior)
{
textBoxControl.TabKeyBehavior = true;
Console.WriteLine("TabKeyBehavior after setting to true: " + textBoxControl.TabKeyBehavior);
}
// Save the workbook
workbook.Save("TextBoxActiveXControlTabKeyBehaviorDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
