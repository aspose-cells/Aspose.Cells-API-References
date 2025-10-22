##TextBoxActiveXControl.IsAutoTab
TextBoxActiveXControl property. Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters
## TextBoxActiveXControl.IsAutoTab property
Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters.
```csharp
public bool IsAutoTab { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyIsAutoTabDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX control and get its control
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 30, 100, 30);
var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
// Demonstrate IsAutoTab property
Console.WriteLine("Initial IsAutoTab value: " + textBoxControl.IsAutoTab);
// Set IsAutoTab to true if it's false
if (!textBoxControl.IsAutoTab)
{
textBoxControl.IsAutoTab = true;
Console.WriteLine("IsAutoTab set to: " + textBoxControl.IsAutoTab);
}
// Save the workbook
workbook.Save("TextBoxActiveXControlIsAutoTabDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
