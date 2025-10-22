##ScrollBarActiveXControl.Type
ScrollBarActiveXControl property. Gets the type of the ActiveX control
## ScrollBarActiveXControl.Type property
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
public class ScrollBarActiveXControlPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ScrollBar ActiveX control with correct parameters
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 1, 1, 100, 20, 0);
ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;
// Check the control type using the Type property
if (scrollBar.Type == ControlType.ScrollBar)
{
// Set ScrollBar specific properties
scrollBar.Max = 100;
scrollBar.Min = 0;
scrollBar.Position = 50;
}
// Save the workbook
workbook.Save("ScrollBarActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
