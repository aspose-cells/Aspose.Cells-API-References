##Enum ControlType
Aspose.Cells.Drawing.ActiveXControls.ControlType enum. Represents all type of ActiveX control
## ControlType enumeration
Represents all type of ActiveX control.
```csharp
public enum ControlType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| CommandButton | `0` | Button |
| ComboBox | `1` | ComboBox |
| CheckBox | `2` | CheckBox |
| ListBox | `3` | ListBox |
| TextBox | `4` | TextBox |
| SpinButton | `5` | Spinner |
| RadioButton | `6` | RadioButton |
| Label | `7` | Label |
| Image | `8` | Image |
| ToggleButton | `9` | ToggleButton |
| ScrollBar | `10` | ScrollBar |
| BarCode | `11` | ScrollBar |
| Unknown | `12` | Unknown |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ControlTypeDemo
{
public static void ControlTypeExample()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CommandButton ActiveX control
Shape commandButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 30);
ActiveXControl commandButtonControl = commandButtonShape.ActiveXControl;
commandButtonControl.IsEnabled = true;
commandButtonControl.IsVisible = true;
// Add a ComboBox ActiveX control
Shape comboBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 1, 0, 100, 30);
ActiveXControl comboBoxControl = comboBoxShape.ActiveXControl;
comboBoxControl.IsEnabled = true;
comboBoxControl.IsVisible = true;
// Add a CheckBox ActiveX control
Shape checkBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 0, 100, 30);
ActiveXControl checkBoxControl = checkBoxShape.ActiveXControl;
checkBoxControl.IsEnabled = true;
checkBoxControl.IsVisible = true;
// Add a ListBox ActiveX control
Shape listBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 7, 0, 1, 0, 100, 30);
ActiveXControl listBoxControl = listBoxShape.ActiveXControl;
listBoxControl.IsEnabled = true;
listBoxControl.IsVisible = true;
// Add a TextBox ActiveX control
Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 9, 0, 1, 0, 100, 30);
ActiveXControl textBoxControl = textBoxShape.ActiveXControl;
textBoxControl.IsEnabled = true;
textBoxControl.IsVisible = true;
// Add a SpinButton ActiveX control
Shape spinButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 11, 0, 1, 0, 100, 30);
ActiveXControl spinButtonControl = spinButtonShape.ActiveXControl;
spinButtonControl.IsEnabled = true;
spinButtonControl.IsVisible = true;
// Add a RadioButton ActiveX control
Shape radioButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 13, 0, 1, 0, 100, 30);
ActiveXControl radioButtonControl = radioButtonShape.ActiveXControl;
radioButtonControl.IsEnabled = true;
radioButtonControl.IsVisible = true;
// Add a Label ActiveX control
Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 15, 0, 1, 0, 100, 30);
ActiveXControl labelControl = labelShape.ActiveXControl;
labelControl.IsEnabled = true;
labelControl.IsVisible = true;
// Add an Image ActiveX control
Shape imageShape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 17, 0, 1, 0, 100, 30);
ActiveXControl imageControl = imageShape.ActiveXControl;
imageControl.IsEnabled = true;
imageControl.IsVisible = true;
// Add a ToggleButton ActiveX control
Shape toggleButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 19, 0, 1, 0, 100, 30);
ActiveXControl toggleButtonControl = toggleButtonShape.ActiveXControl;
toggleButtonControl.IsEnabled = true;
toggleButtonControl.IsVisible = true;
// Add a ScrollBar ActiveX control
Shape scrollBarShape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 21, 0, 1, 0, 100, 30);
ActiveXControl scrollBarControl = scrollBarShape.ActiveXControl;
scrollBarControl.IsEnabled = true;
scrollBarControl.IsVisible = true;
// Save the workbook
workbook.Save("ControlTypeExample.xlsx");
workbook.Save("ControlTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
