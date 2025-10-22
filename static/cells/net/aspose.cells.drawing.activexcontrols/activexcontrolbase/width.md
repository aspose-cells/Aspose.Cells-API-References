##ActiveXControlBase.Width
ActiveXControlBase property. Gets and sets the width of the control in unit of points
## ActiveXControlBase.Width property
Gets and sets the width of the control in unit of points.
```csharp
public virtual double Width { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
ActiveXControlBase control = (ActiveXControlBase)shape.ActiveXControl;
// Demonstrate Width property usage
Console.WriteLine("Original width: " + control.Width);
control.Width = 150;
Console.WriteLine("Modified width: " + control.Width);
workbook.Save("ActiveXControlWidthDemo.xlsx");
}
}
}
```
### See Also
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
