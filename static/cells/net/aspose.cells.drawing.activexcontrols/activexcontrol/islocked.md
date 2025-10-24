##ActiveXControl.IsLocked
ActiveXControl property. Indicates whether data in the control is locked for editing
## ActiveXControl.IsLocked property
Indicates whether data in the control is locked for editing.
```csharp
public bool IsLocked { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlPropertyIsLockedDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Unlock all columns except first
Style style;
StyleFlag flag;
for (int i = 0; i <= 255; i++)
{
style = sheet.Cells.Columns[(byte)i].GetStyle();
style.IsLocked = false;
flag = new StyleFlag();
flag.Locked = true;
sheet.Cells.Columns[(byte)i].ApplyStyle(style, flag);
}
// Lock first column
style = sheet.Cells.Columns[0].GetStyle();
style.IsLocked = true;
flag = new StyleFlag();
flag.Locked = true;
sheet.Cells.Columns[0].ApplyStyle(style, flag);
// Add ActiveX ComboBox control
Shape comboBoxShape = sheet.Shapes.AddActiveXControl(
ControlType.ComboBox,
5, 0, 5, 0, 100, 20);
// Set ActiveX control properties including IsLocked
ComboBoxActiveXControl comboBox =
(ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
comboBox.IsLocked = false; // Demonstrate IsLocked property
comboBox.IsVisible = true;
comboBox.BorderStyle = ControlBorderType.None;
// Protect the worksheet
sheet.Protect(ProtectionType.All);
// Save the workbook
wb.Save("ActiveXControlIsLockedDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
