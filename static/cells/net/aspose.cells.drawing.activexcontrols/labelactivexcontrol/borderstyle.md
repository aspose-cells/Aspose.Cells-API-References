##LabelActiveXControl.BorderStyle
LabelActiveXControl property. Gets and set the type of border used by the control
## LabelActiveXControl.BorderStyle property
Gets and set the type of border used by the control.
```csharp
public ControlBorderType BorderStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class LabelActiveXControlPropertyBorderStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;
label.Caption = "Border Style Demo";
label.BorderStyle = ControlBorderType.Single;
label.BorderOleColor = 0xFF0000; // Red border
Console.WriteLine("Label Border Style: " + label.BorderStyle);
Console.WriteLine("Label Border Color: " + label.BorderOleColor);
workbook.Save("LabelBorderStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlBorderType](../../controlbordertype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
