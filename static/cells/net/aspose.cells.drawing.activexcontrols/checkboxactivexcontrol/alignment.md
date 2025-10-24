##CheckBoxActiveXControl.Alignment
CheckBoxActiveXControl property. Gets and set the position of the Caption relative to the control
## CheckBoxActiveXControl.Alignment property
Gets and set the position of the Caption relative to the control.
```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CheckBoxActiveXControlPropertyAlignmentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 30);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
checkBox.Caption = "Sample CheckBox";
checkBox.Alignment = ControlCaptionAlignmentType.Right;
checkBox.IsWordWrapped = true;
checkBox.Value = CheckValueType.Checked;
workbook.Save("CheckBoxAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
