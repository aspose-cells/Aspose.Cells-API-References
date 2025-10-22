##Enum DropButtonStyle
Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle enum. Represents the symbol displayed on the drop button
## DropButtonStyle enumeration
Represents the symbol displayed on the drop button.
```csharp
public enum DropButtonStyle
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Plain | `0` | Displays a button with no symbol. |
| Arrow | `1` | Displays a button with a down arrow. |
| Ellipsis | `2` | Displays a button with an ellipsis (...). |
| Reduce | `3` | Displays a button with a horizontal line like an underscore character. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class DropButtonStyleDemo
{
public static void DropButtonStyleExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ComboBox
comboBox.ListWidth = 100;
comboBox.ListRows = 5;
comboBox.ColumnCount = 1;
comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow
// Add some items to the ComboBox
comboBox.LinkedCell = "A1";
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
worksheet.Cells["A4"].PutValue("Item 4");
comboBox.ListFillRange = "A1:A4";
// Save the workbook
workbook.Save("DropButtonStyleExample.xlsx");
workbook.Save("DropButtonStyleExample.pdf");
// Output the DropButtonStyle used
Console.WriteLine("DropButtonStyle set to: " + comboBox.DropButtonStyle);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
