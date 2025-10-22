##Enum ControlSpecialEffectType
Aspose.Cells.Drawing.ActiveXControls.ControlSpecialEffectType enum. Represents the type of special effect
## ControlSpecialEffectType enumeration
Represents the type of special effect.
```csharp
public enum ControlSpecialEffectType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Flat | `0` | Flat |
| Raised | `1` | Raised |
| Sunken | `2` | Sunken |
| Etched | `3` | Etched |
| Bump | `6` | Bump |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ControlSpecialEffectTypeDemo
{
public static void ControlSpecialEffectTypeExample()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;
// Set properties of the CheckBox ActiveX control
checkBoxControl.Caption = "Example CheckBox";
checkBoxControl.SpecialEffect = ControlSpecialEffectType.Raised;
// Add a ComboBox ActiveX control
shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 3, 0, 100, 50);
ComboBoxActiveXControl comboBoxControl = (ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties of the ComboBox ActiveX control
comboBoxControl.SpecialEffect = ControlSpecialEffectType.Sunken;
comboBoxControl.ListWidth = 100;
comboBoxControl.ListRows = 5;
// Add a TextBox ActiveX control
shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 5, 0, 5, 0, 100, 50);
TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;
// Set properties of the TextBox ActiveX control
textBoxControl.Text = "Example TextBox";
textBoxControl.SpecialEffect = ControlSpecialEffectType.Bump;
// Save the workbook
workbook.Save("ControlSpecialEffectTypeExample.xlsx");
workbook.Save("ControlSpecialEffectTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
