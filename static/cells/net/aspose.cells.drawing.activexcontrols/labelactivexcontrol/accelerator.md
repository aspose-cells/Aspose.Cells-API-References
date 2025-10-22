##LabelActiveXControl.Accelerator
LabelActiveXControl property. Gets and sets the accelerator key for the control
## LabelActiveXControl.Accelerator property
Gets and sets the accelerator key for the control.
```csharp
public char Accelerator { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class LabelActiveXControlPropertyAcceleratorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;
label.Caption = "Press Alt+H";
label.Accelerator = 'H';
label.IsVisible = true;
Console.WriteLine("Label Caption: " + label.Caption);
Console.WriteLine("Label Accelerator: " + label.Accelerator);
workbook.Save("LabelActiveXControlAcceleratorDemo.xlsx");
}
}
}
```
### See Also
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
