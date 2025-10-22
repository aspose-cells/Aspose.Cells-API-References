##ComboBoxActiveXControl.ShowDropButtonTypeWhen
ComboBoxActiveXControl property. Specifies the symbol displayed on the drop button
## ComboBoxActiveXControl.ShowDropButtonTypeWhen property
Specifies the symbol displayed on the drop button
```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
5, 0, 100, 20, 100, 20);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox =
(Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
comboBox.ShowDropButtonTypeWhen = Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType.Always;
comboBox.DropButtonStyle = Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle.Arrow;
comboBox.Value = "Click the drop button";
workbook.Save("ComboBoxShowDropButtonDemo.xlsx");
}
}
}
```
### See Also
* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
