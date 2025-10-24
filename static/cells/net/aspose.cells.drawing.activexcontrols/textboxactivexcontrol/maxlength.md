##TextBoxActiveXControl.MaxLength
TextBoxActiveXControl property. Gets and sets the maximum number of characters
## TextBoxActiveXControl.MaxLength property
Gets and sets the maximum number of characters
```csharp
public int MaxLength { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyMaxLengthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX Control and get its ActiveXControl property
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Set MaxLength property
if (textBox.MaxLength == 0)
{
textBox.MaxLength = 30;
}
// Save the workbook
workbook.Save("TextBoxMaxLengthDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
