##ActiveXControl.IsTransparent
ActiveXControl property. Indicates whether the control is transparent
## ActiveXControl.IsTransparent property
Indicates whether the control is transparent.
```csharp
public bool IsTransparent { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlPropertyIsTransparentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to host the ActiveX control with all required parameters
Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.Label,
1, 1, 200, 50,
0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top
LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;
// Set control properties
label.Caption = "Sample Label";
label.IsTransparent = false; // Demonstrating IsTransparent property
// Verify and output the IsTransparent property
Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);
// Change transparency and verify again
label.IsTransparent = true;
Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);
// Save the workbook
workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
}
}
}
```
### See Also
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
