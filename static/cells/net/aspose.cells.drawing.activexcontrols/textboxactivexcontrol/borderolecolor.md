##TextBoxActiveXControl.BorderOleColor
TextBoxActiveXControl property. Gets and sets the ole color of the background
## TextBoxActiveXControl.BorderOleColor property
Gets and sets the ole color of the background.
```csharp
public int BorderOleColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyBorderOleColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an ActiveX TextBox control and get its ActiveXControl property
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 100, 100, 100);
var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Set the BorderOleColor property (Excel default color system 12 or green)
textBox.BorderOleColor = unchecked((int)0x80000012);
// Save the workbook
workbook.Save("TextBoxActiveXControlBorderOleColorDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
