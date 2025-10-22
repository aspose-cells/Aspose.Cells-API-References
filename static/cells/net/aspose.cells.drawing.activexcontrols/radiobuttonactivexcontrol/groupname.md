##RadioButtonActiveXControl.GroupName
RadioButtonActiveXControl property. Gets and sets the groups name
## RadioButtonActiveXControl.GroupName property
Gets and sets the group's name.
```csharp
public string GroupName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RadioButtonActiveXControlPropertyGroupNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add two RadioButton ActiveX controls
var shape1 = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
var shape2 = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;
// Set the same group name to make them mutually exclusive
radio1.GroupName = "RadioGroup1";
radio2.GroupName = "RadioGroup1";
// Set captions
radio1.Caption = "Option 1";
radio2.Caption = "Option 2";
// Save the workbook
workbook.Save("RadioButtonGroupDemo.xlsx");
}
}
}
```
### See Also
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
