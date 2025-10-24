##CommandButtonActiveXControl.Caption
CommandButtonActiveXControl property. Gets and set the descriptive text that appears on a control
## CommandButtonActiveXControl.Caption property
Gets and set the descriptive text that appears on a control.
```csharp
public string Caption { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class CommandButtonActiveXControlPropertyCaptionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl commandButton = (Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl)shape.ActiveXControl;
// Demonstrate Caption property usage
commandButton.Caption = "Click Me";
commandButton.Width = 150;
commandButton.Height = 50;
commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
workbook.Save("CommandButtonCaptionDemo.xlsx");
}
}
}
```
### See Also
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
