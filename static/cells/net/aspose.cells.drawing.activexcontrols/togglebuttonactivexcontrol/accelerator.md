##ToggleButtonActiveXControl.Accelerator
ToggleButtonActiveXControl property. Gets and sets the accelerator key for the control
## ToggleButtonActiveXControl.Accelerator property
Gets and sets the accelerator key for the control.
```csharp
public char Accelerator { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ToggleButtonActiveXControlPropertyAcceleratorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ToggleButton ActiveX control with proper parameters
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;
// Set the Accelerator property
toggleButton.Accelerator = 'A';
Console.WriteLine("ToggleButton Accelerator set to: " + toggleButton.Accelerator);
// Clear the Accelerator property
toggleButton.Accelerator = '\0';
Console.WriteLine("ToggleButton Accelerator cleared: " + (toggleButton.Accelerator == '\0' ? "True" : "False"));
}
}
}
```
### See Also
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
