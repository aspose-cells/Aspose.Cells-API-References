##ComboBoxActiveXControl.Type
ComboBoxActiveXControl property. Gets the type of the ActiveX control
## ComboBoxActiveXControl.Type property
Gets the type of the ActiveX control.
```csharp
public override ControlType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape comboBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
comboBox.ListWidth = 0;
comboBox.BoundColumn = 1;
comboBox.TextColumn = -1;
Console.WriteLine("Control Type: " + comboBox.Type);
workbook.Save("ComboBoxActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
