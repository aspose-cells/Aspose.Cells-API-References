##TextBoxActiveXControl.HideSelection
TextBoxActiveXControl property. Indicates whether selected text in the control appears highlighted when the control does not have focus
## TextBoxActiveXControl.HideSelection property
Indicates whether selected text in the control appears highlighted when the control does not have focus.
```csharp
public bool HideSelection { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyHideSelectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an ActiveX TextBox control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Demonstrate HideSelection property
Console.WriteLine("Initial HideSelection value: " + textBox.HideSelection);
// Set HideSelection to true if it's false
if (!textBox.HideSelection)
{
textBox.HideSelection = true;
Console.WriteLine("HideSelection set to: " + textBox.HideSelection);
}
// Save the workbook
workbook.Save("TextBoxActiveXControlHideSelectionDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
