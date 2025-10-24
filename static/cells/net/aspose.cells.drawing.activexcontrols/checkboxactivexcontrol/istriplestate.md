##CheckBoxActiveXControl.IsTripleState
CheckBoxActiveXControl property. Indicates how the specified control will display Null values
## CheckBoxActiveXControl.IsTripleState property
Indicates how the specified control will display Null values.
```csharp
public bool IsTripleState { get; set; }
```
### Remarks
| **Setting** | **Description** |
| --- | --- |
| True | The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null. |
| False | (Default) The control will cycle through states for Yes and No values. Null values display as if they were No values. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CheckBoxActiveXControlPropertyIsTripleStateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
// Configure basic properties
checkBox.Caption = "Triple State Demo";
// Demonstrate IsTripleState property
checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state
// Save the workbook
workbook.Save("CheckBoxTripleStateDemo.xlsx");
}
}
}
```
### See Also
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
