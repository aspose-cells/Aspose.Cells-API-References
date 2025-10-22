##CommandButtonActiveXControl.Type
CommandButtonActiveXControl property. Gets the type of the ActiveX control
## CommandButtonActiveXControl.Type property
Gets the type of the ActiveX control.
```csharp
public override ControlType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CommandButtonActiveXControlPropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create command button with full parameter list
Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.CommandButton,
0,  // topRow
0,  // top
0,  // leftColumn
0,  // left
100,  // width
100  // height
);
var control = (CommandButtonActiveXControl)shape.ActiveXControl;
control.Caption = "CommandButton1";
control.PicturePosition = ControlPicturePositionType.AboveCenter;
control.Accelerator = (char)0;
control.TakeFocusOnClick = false;
control.IsWordWrapped = false;
control.IsEnabled = true;
Console.WriteLine($"Control Type: {control.Type}");
Console.WriteLine($"Is CommandButton type: {control.Type == ControlType.CommandButton}");
workbook.Save("CommandButtonDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
