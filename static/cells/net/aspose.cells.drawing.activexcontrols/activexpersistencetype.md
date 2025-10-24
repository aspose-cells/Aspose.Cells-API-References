##Enum ActiveXPersistenceType
Aspose.Cells.Drawing.ActiveXControls.ActiveXPersistenceType enum. Represents the persistence method to persist an ActiveX control
## ActiveXPersistenceType enumeration
Represents the persistence method to persist an ActiveX control.
```csharp
public enum ActiveXPersistenceType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| PropertyBag | `0` | The data is stored as xml data. |
| Storage | `1` | The data is stored as a storage binary data. |
| Stream | `2` | The data is stored as a stream binary data. |
| StreamInit | `3` | The data is stored as a streaminit binary data. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ActiveXControlsClassActiveXPersistenceTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
cells["A2"].Value = "Sales";
cells["A3"].Value = "Finance";
cells["A4"].Value = "MIS";
cells["A5"].Value = "R&D";
cells["A6"].Value = "Marketing";
cells["A7"].Value = "HRA";
// Add different ActiveX controls to demonstrate various persistence types
AddControlWithPersistenceType(worksheet, ControlType.CommandButton, ActiveXPersistenceType.PropertyBag, 0, 2);
AddControlWithPersistenceType(worksheet, ControlType.TextBox, ActiveXPersistenceType.Storage, 4, 2);
AddControlWithPersistenceType(worksheet, ControlType.CheckBox, ActiveXPersistenceType.Stream, 8, 2);
AddControlWithPersistenceType(worksheet, ControlType.ComboBox, ActiveXPersistenceType.StreamInit, 12, 2);
// Save the workbook with all ActiveX controls
workbook.Save("ActiveXPersistenceTypeDemo.xlsx");
}
private static void AddControlWithPersistenceType(Worksheet worksheet, ControlType controlType,
ActiveXPersistenceType persistenceType, int row, int column)
{
// Add an ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(
controlType,
row,
15,
column,
15,
200,
50
);
// Configure control based on type
switch (controlType)
{
case ControlType.CommandButton:
var button = (CommandButtonActiveXControl)shape.ActiveXControl;
button.IsVisible = true;
button.Caption = $"{persistenceType} Button";
break;
case ControlType.TextBox:
var textBox = (TextBoxActiveXControl)shape.ActiveXControl;
textBox.IsVisible = true;
textBox.Text = $"{persistenceType} TextBox";
break;
case ControlType.CheckBox:
var checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
checkBox.IsVisible = true;
checkBox.Caption = $"{persistenceType} CheckBox";
checkBox.Value = CheckValueType.Checked;
break;
case ControlType.ComboBox:
var comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
comboBox.IsVisible = true;
comboBox.ListFillRange = $"A3:A7";
break;
}
// The persistence type is handled internally by Aspose.Cells when saving
Console.WriteLine($"Added {controlType} with persistence type: {persistenceType}");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
