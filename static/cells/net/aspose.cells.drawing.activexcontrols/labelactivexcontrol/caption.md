##LabelActiveXControl.Caption
LabelActiveXControl property. Gets and set the descriptive text that appears on a control
## LabelActiveXControl.Caption property
Gets and set the descriptive text that appears on a control.
```csharp
public string Caption { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class LabelActiveXControlPropertyCaptionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add Label ActiveX Control
Shape shape = sheet.Shapes.AddActiveXControl(ControlType.Label, 0, 0, 0, 0, 100, 30);
LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;
// Set and demonstrate Caption property
label.Caption = "Label1aaaa";
// Save and reload to verify persistence
string path = "LabelActiveXDemo.xlsm";
workbook.Save(path, SaveFormat.Xlsm);
Workbook reopened = new Workbook(path);
LabelActiveXControl reloadedLabel = (LabelActiveXControl)reopened.Worksheets[0].Shapes[0].ActiveXControl;
Console.WriteLine("Caption: " + reloadedLabel.Caption);
}
}
}
```
### See Also
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
