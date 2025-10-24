##CheckBoxActiveXControl.GroupName
CheckBoxActiveXControl property. Gets and sets the groups name
## CheckBoxActiveXControl.GroupName property
Gets and sets the group's name.
```csharp
public string GroupName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CheckBoxActiveXControlPropertyGroupNameDemo
{
public static void Run()
{
// Create workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
// Set GroupName property
checkBox.GroupName = "Sheet1";
// Verify and output the GroupName
Console.WriteLine("CheckBox GroupName: " + checkBox.GroupName);
// Save the workbook
workbook.Save("CheckBoxActiveXControlGroupNameDemo.xlsx");
}
}
}
```
### See Also
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
