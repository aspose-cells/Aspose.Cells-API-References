##RadioButtonActiveXControl.IsWordWrapped
RadioButtonActiveXControl property. Indicates whether the contents of the control automatically wrap at the end of a line
## RadioButtonActiveXControl.IsWordWrapped property
Indicates whether the contents of the control automatically wrap at the end of a line.
```csharp
public bool IsWordWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class RadioButtonActiveXControlPropertyIsWordWrappedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a RadioButton ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton,
1, 1, 100, 50, 100, 50);
Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl radioButton =
(Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape.ActiveXControl;
// Demonstrate IsWordWrapped property
Console.WriteLine("Initial IsWordWrapped value: " + radioButton.IsWordWrapped);
radioButton.IsWordWrapped = true;
Console.WriteLine("After setting IsWordWrapped to true: " + radioButton.IsWordWrapped);
radioButton.IsWordWrapped = false;
Console.WriteLine("After setting IsWordWrapped to false: " + radioButton.IsWordWrapped);
// Save the workbook
workbook.Save("RadioButtonIsWordWrappedDemo.xlsx");
}
}
}
```
### See Also
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
