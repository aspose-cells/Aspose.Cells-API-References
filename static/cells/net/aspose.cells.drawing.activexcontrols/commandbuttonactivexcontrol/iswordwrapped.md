##CommandButtonActiveXControl.IsWordWrapped
CommandButtonActiveXControl property. Indicates whether the contents of the control automatically wrap at the end of a line
## CommandButtonActiveXControl.IsWordWrapped property
Indicates whether the contents of the control automatically wrap at the end of a line.
```csharp
public bool IsWordWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CommandButtonActiveXControlPropertyIsWordWrappedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 0, 0, 2, 2, 150, 30);
CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;
button.Caption = "Click to demonstrate word wrapping in caption";
button.IsWordWrapped = true;
workbook.Save("CommandButtonIsWordWrappedDemo.xlsm");
}
}
}
```
### See Also
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
