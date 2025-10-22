##LabelActiveXControl.BorderOleColor
LabelActiveXControl property. Gets and sets the ole color of the background
## LabelActiveXControl.BorderOleColor property
Gets and sets the ole color of the background.
```csharp
public int BorderOleColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LabelActiveXControlPropertyBorderOleColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a Label ActiveX Control
Shape shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 1, 0, 1, 0, 100, 50);
Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl labelControl =
(Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;
// Set properties
labelControl.Caption = "Sample Label";
labelControl.BorderOleColor = -2147483642; // Set border color (OLE_COLOR)
labelControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
// Save the workbook
workbook.Save("LabelActiveXControlBorderOleColorDemo.xlsx");
// Display the border color
Console.WriteLine("BorderOleColor: " + labelControl.BorderOleColor);
}
}
}
```
### See Also
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
