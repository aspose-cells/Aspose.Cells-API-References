##CheckBoxActiveXControl.Caption
CheckBoxActiveXControl property. Gets and set the descriptive text that appears on a control
## CheckBoxActiveXControl.Caption property
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
public class CheckBoxActiveXControlPropertyCaptionDemo
{
public static void Run()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;
// Set and demonstrate the Caption property
checkBoxControl.Caption = "Sample CheckBox Caption";
checkBoxControl.Value = CheckValueType.Checked;  // Fixed: Using correct enum value
// Save the workbook
workbook.Save("CheckBoxCaptionDemo.xlsx");
}
}
}
```
### See Also
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
