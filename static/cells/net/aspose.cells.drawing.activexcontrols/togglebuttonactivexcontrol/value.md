##ToggleButtonActiveXControl.Value
ToggleButtonActiveXControl property. Indicates if the control is checked or not
## ToggleButtonActiveXControl.Value property
Indicates if the control is checked or not.
```csharp
public CheckValueType Value { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ToggleButtonActiveXControlPropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ToggleButton ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;
// Set initial value to Unchecked
toggleButton.Value = CheckValueType.UnChecked;
// Check and toggle the value if it's Unchecked
if (toggleButton.Value == CheckValueType.UnChecked)
{
toggleButton.Value = CheckValueType.Checked;
}
// Save the workbook
workbook.Save("ToggleButtonDemo.xlsx");
}
}
}
```
### See Also
* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
