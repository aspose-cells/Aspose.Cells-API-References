##ToggleButtonActiveXControl.IsTripleState
ToggleButtonActiveXControl property. Indicates how the specified control will display Null values
## ToggleButtonActiveXControl.IsTripleState property
Indicates how the specified control will display Null values.
```csharp
public bool IsTripleState { get; set; }
```
### Remarks
| **Setting** | **Description** |
| --- | --- |
| True | The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null. |
| False | (Default) The control will cycle through states for Yes and No values. Null values display as if they were No values. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ToggleButton ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;
// Set IsTripleState property to true
toggleButton.IsTripleState = true;
Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);
// Change IsTripleState property to false
toggleButton.IsTripleState = false;
Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);
// Save the workbook
workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
}
}
}
```
### See Also
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
