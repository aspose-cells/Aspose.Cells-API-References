##ComboBoxActiveXControl.SpecialEffect
ComboBoxActiveXControl property. Gets and sets the special effect of the control
## ComboBoxActiveXControl.SpecialEffect property
Gets and sets the special effect of the control.
```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertySpecialEffectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(
ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
var control = (ComboBoxActiveXControl)shape.ActiveXControl;
control.SpecialEffect = ControlSpecialEffectType.Sunken;
control.ListRows = 8;
control.ColumnCount = 1;
workbook.Save("output.xls", SaveFormat.Excel97To2003);
}
}
}
```
### See Also
* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
