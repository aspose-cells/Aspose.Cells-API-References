##ActiveXControlBase.Shadow
ActiveXControlBase property. Indicates whether to show a shadow
## ActiveXControlBase.Shadow property
Indicates whether to show a shadow.
```csharp
public virtual bool Shadow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyShadowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;
commandButton.Caption = "Shadow Button";
commandButton.Shadow = true;
workbook.Save("ActiveXControlShadowDemo.xlsx");
}
}
}
```
### See Also
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
