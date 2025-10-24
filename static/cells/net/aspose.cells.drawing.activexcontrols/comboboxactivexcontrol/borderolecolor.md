##ComboBoxActiveXControl.BorderOleColor
ComboBoxActiveXControl property. Gets and sets the ole color of the background
## ComboBoxActiveXControl.BorderOleColor property
Gets and sets the ole color of the background.
```csharp
public int BorderOleColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyBorderOleColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
1, 1, 100, 20, 100, 20);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox =
(Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Configure basic properties
comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
// Demonstrate BorderOleColor property
comboBox.BorderOleColor = ColorTranslator.ToOle(Color.Red); // Set border color to red
// Set some sample text
comboBox.Value = "Border Color Demo";
// Save the workbook
workbook.Save("ComboBoxBorderColorDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
