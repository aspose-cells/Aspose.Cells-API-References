##TextBoxActiveXControl.IntegralHeight
TextBoxActiveXControl property. Indicates whether the control will only show complete lines of text without showing any partial lines
## TextBoxActiveXControl.IntegralHeight property
Indicates whether the control will only show complete lines of text without showing any partial lines.
```csharp
public bool IntegralHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyIntegralHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an ActiveX TextBox control and get its ActiveXControl property
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Demonstrate IntegralHeight property
Console.WriteLine("Initial IntegralHeight: " + textBox.IntegralHeight);
// Set IntegralHeight to true if it's false
if (!textBox.IntegralHeight)
{
textBox.IntegralHeight = true;
Console.WriteLine("IntegralHeight set to: " + textBox.IntegralHeight);
}
// Save the workbook
workbook.Save("TextBoxActiveXControlIntegralHeightDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
