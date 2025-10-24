##TextBoxActiveXControl.IsDragBehaviorEnabled
TextBoxActiveXControl property. Indicates whether dragging and dropping is enabled for the control
## TextBoxActiveXControl.IsDragBehaviorEnabled property
Indicates whether dragging and dropping is enabled for the control.
```csharp
public bool IsDragBehaviorEnabled { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyIsDragBehaviorEnabledDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 22);
TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
if (!textBox.IsDragBehaviorEnabled)
{
textBox.IsDragBehaviorEnabled = true;
}
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
