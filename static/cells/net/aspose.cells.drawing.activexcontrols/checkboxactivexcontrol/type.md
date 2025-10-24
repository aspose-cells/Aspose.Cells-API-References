##CheckBoxActiveXControl.Type
CheckBoxActiveXControl property. Gets the type of the ActiveX control
## CheckBoxActiveXControl.Type property
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
public class CheckBoxActiveXControlPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
// Set properties
checkBox.Caption = "Sample CheckBox";
checkBox.GroupName = "Sheet1";
checkBox.Alignment = ControlCaptionAlignmentType.Right;
checkBox.IsWordWrapped = true;
checkBox.Value = CheckValueType.UnChecked;
checkBox.IsEnabled = true;
// Demonstrate Type property usage
Console.WriteLine("Control Type: " + checkBox.Type); // Output: Control Type: CheckBox
if (checkBox.Type == ControlType.CheckBox)
{
Console.WriteLine("This is a CheckBox control");
}
// Save the workbook
workbook.Save("CheckBoxActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
