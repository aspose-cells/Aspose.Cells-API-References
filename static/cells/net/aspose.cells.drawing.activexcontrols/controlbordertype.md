##Enum ControlBorderType
Aspose.Cells.Drawing.ActiveXControls.ControlBorderType enum. Represents the border type of the ActiveX control
## ControlBorderType enumeration
Represents the border type of the ActiveX control.
```csharp
public enum ControlBorderType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No border. |
| Single | `1` | The single line. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
public class ControlBorderTypeDemo
{
public static void ControlBorderTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ComboBox ActiveX control
comboBox.MaxLength = 100;
comboBox.ListWidth = 150;
comboBox.BoundColumn = 1;
comboBox.TextColumn = 1;
comboBox.ColumnCount = 1;
comboBox.ListRows = 5;
comboBox.MatchEntry = ControlMatchEntryType.Complete;
comboBox.DropButtonStyle = DropButtonStyle.Arrow;
comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Always;
comboBox.ListStyle = ControlListStyle.Plain;
comboBox.BorderStyle = ControlBorderType.Single; // Set border style to Single
comboBox.BorderOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
comboBox.SpecialEffect = ControlSpecialEffectType.Flat;
comboBox.IsEditable = true;
comboBox.ShowColumnHeads = false;
comboBox.IsDragBehaviorEnabled = false;
comboBox.EnterFieldBehavior = true;
comboBox.IsAutoWordSelected = false;
comboBox.SelectionMargin = false;
comboBox.Value = "Sample Text";
comboBox.HideSelection = true;
comboBox.ColumnWidths = 100;
// Save the workbook
workbook.Save("ControlBorderTypeExample.xlsx");
workbook.Save("ControlBorderTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
