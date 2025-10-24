##LabelActiveXControl.Type
LabelActiveXControl property. Gets the type of the ActiveX control
## LabelActiveXControl.Type property
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
public class LabelActiveXControlPropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 200, 50, 0, 0);
LabelActiveXControl labelControl = (LabelActiveXControl)labelShape.ActiveXControl;
labelControl.Caption = "Demo Label";
Console.WriteLine("Label Control Type: " + labelControl.Type);
workbook.Save("LabelControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
