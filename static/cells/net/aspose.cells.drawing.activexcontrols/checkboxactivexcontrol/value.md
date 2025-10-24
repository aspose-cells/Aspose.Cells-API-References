##CheckBoxActiveXControl.Value
CheckBoxActiveXControl property. Indicates if the control is checked or not
## CheckBoxActiveXControl.Value property
Indicates if the control is checked or not.
```csharp
public CheckValueType Value { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CheckBoxActiveXControlPropertyValueDemo
{
public static void Run()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
// Set basic properties including Value
checkBox.Caption = "Check Me";
checkBox.Value = CheckValueType.Checked; // Demonstrating Value property usage
// Save the workbook
workbook.Save("CheckBoxActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
