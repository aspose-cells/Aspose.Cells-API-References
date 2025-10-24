##LabelActiveXControl.IsWordWrapped
LabelActiveXControl property. Indicates whether the contents of the control automatically wrap at the end of a line
## LabelActiveXControl.IsWordWrapped property
Indicates whether the contents of the control automatically wrap at the end of a line.
```csharp
public bool IsWordWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LabelActiveXControlPropertyIsWordWrappedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 5, 0, 1, 1, 100, 20);
Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl label = (Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;
label.Caption = "This is a long text that will demonstrate word wrapping when IsWordWrapped is set to true";
label.IsWordWrapped = true;
label.IsAutoSize = true;
Console.WriteLine("Label IsWordWrapped: " + label.IsWordWrapped);
Console.WriteLine("Label Caption: " + label.Caption);
workbook.Save("LabelActiveXControlIsWordWrappedDemo.xlsx");
}
}
}
```
### See Also
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
