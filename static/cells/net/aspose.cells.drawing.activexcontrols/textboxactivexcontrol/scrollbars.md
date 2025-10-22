##TextBoxActiveXControl.ScrollBars
TextBoxActiveXControl property. Indicates specifies whether the control has vertical scroll bars horizontal scroll bars both or neither
## TextBoxActiveXControl.ScrollBars property
Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither.
```csharp
public ControlScrollBarType ScrollBars { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyScrollBarsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a new shape collection and add ActiveX control
ShapeCollection shapes = worksheet.Shapes;
Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
// Set the ScrollBars property to vertical
textBox.ScrollBars = ControlScrollBarType.BarsVertical;
// Save the workbook
workbook.Save("TextBoxScrollBarsDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
