##ActiveXControlBase.MousePointer
ActiveXControlBase property. Gets and sets the type of icon displayed as the mouse pointer for the control
## ActiveXControlBase.MousePointer property
Gets and sets the type of icon displayed as the mouse pointer for the control.
```csharp
public ControlMousePointerType MousePointer { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyMousePointerDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 50);
CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;
button.Caption = "Click Me";
button.MousePointer = ControlMousePointerType.Help;
button.MouseIcon = new byte[] { }; // Empty byte array for custom icon (when MousePointer is Custom)
workbook.Save("ActiveXControlMousePointerDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlMousePointerType](../../controlmousepointertype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
