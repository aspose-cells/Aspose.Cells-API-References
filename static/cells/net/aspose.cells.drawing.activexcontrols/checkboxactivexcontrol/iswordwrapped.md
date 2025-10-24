##CheckBoxActiveXControl.IsWordWrapped
CheckBoxActiveXControl property. Indicates whether the contents of the control automatically wrap at the end of a line
## CheckBoxActiveXControl.IsWordWrapped property
Indicates whether the contents of the control automatically wrap at the end of a line.
```csharp
public bool IsWordWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class CheckBoxActiveXControlPropertyIsWordWrappedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 150, 50);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
checkBox.Caption = "This is a long caption that should word wrap when enabled";
checkBox.IsWordWrapped = true;
checkBox.IsAutoSize = true;
workbook.Save("CheckBoxWordWrapDemo.xlsx");
}
}
}
```
### See Also
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
