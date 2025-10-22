##CommandButtonActiveXControl.TakeFocusOnClick
CommandButtonActiveXControl property. Indicates whether the control takes the focus when clicked
## CommandButtonActiveXControl.TakeFocusOnClick property
Indicates whether the control takes the focus when clicked.
```csharp
public bool TakeFocusOnClick { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CommandButtonActiveXControlPropertyTakeFocusOnClickDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;
commandButton.Caption = "Click Me";
commandButton.TakeFocusOnClick = true;
workbook.Save("CommandButtonActiveXControlTakeFocusOnClickDemo.xlsx");
}
}
}
```
### See Also
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
