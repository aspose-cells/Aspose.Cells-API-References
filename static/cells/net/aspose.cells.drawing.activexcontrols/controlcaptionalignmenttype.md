##Enum ControlCaptionAlignmentType
Aspose.Cells.Drawing.ActiveXControls.ControlCaptionAlignmentType enum. Represents the position of the Caption relative to the control
## ControlCaptionAlignmentType enumeration
Represents the position of the Caption relative to the control.
```csharp
public enum ControlCaptionAlignmentType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Left | `0` | The left of the control. |
| Right | `1` | The right of the control. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ControlCaptionAlignmentTypeDemo
{
public static void ControlCaptionAlignmentTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 1, 100, 20);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
// Set properties for the CheckBox
checkBox.Caption = "Check Me!";
checkBox.Alignment = ControlCaptionAlignmentType.Right;
checkBox.IsWordWrapped = true;
checkBox.Value = CheckValueType.Checked;
// Add a RadioButton ActiveX control to the worksheet
var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 10, 0, 1, 1, 100, 20);
RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape2.ActiveXControl;
// Set properties for the RadioButton
radioButton.Caption = "Select Me!";
radioButton.Alignment = ControlCaptionAlignmentType.Left;
radioButton.IsWordWrapped = true;
// Save the workbook
workbook.Save("ControlCaptionAlignmentTypeExample.xlsx");
workbook.Save("ControlCaptionAlignmentTypeExample.pdf");
// Output the results
Console.WriteLine("CheckBox Alignment: " + checkBox.Alignment);
Console.WriteLine("RadioButton Alignment: " + radioButton.Alignment);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
