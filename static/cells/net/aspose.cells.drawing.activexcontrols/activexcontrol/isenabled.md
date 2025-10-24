##ActiveXControl.IsEnabled
ActiveXControl property. Indicates whether the control can receive the focus and respond to usergenerated events
## ActiveXControl.IsEnabled property
Indicates whether the control can receive the focus and respond to user-generated events.
```csharp
public bool IsEnabled { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlPropertyIsEnabledDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 1, 0, 1, 100, 50);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
checkBox.IsEnabled = true;
checkBox.GroupName = "Sheet1";
checkBox.Alignment = ControlCaptionAlignmentType.Right;
checkBox.IsWordWrapped = true;
checkBox.Value = CheckValueType.UnChecked;
Console.WriteLine("IsEnabled state: " + checkBox.IsEnabled);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
