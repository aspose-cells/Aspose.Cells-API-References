##Enum ShowDropButtonType
Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType enum. Specifies when to show the drop button
## ShowDropButtonType enumeration
Specifies when to show the drop button
```csharp
public enum ShowDropButtonType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Never | `0` | Never show the drop button. |
| Focus | `1` | Show the drop button when the control has the focus. |
| Always | `2` | Always show the drop button. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ShowDropButtonTypeDemo
{
public static void ShowDropButtonTypeExample()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control to the worksheet
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ComboBox ActiveX control
comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
comboBox.ListWidth = 100;
comboBox.ListRows = 5;
comboBox.IsEditable = true;
// Add some items to the ComboBox
comboBox.LinkedCell = "A1";
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
// Save the workbook
workbook.Save("ShowDropButtonTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
