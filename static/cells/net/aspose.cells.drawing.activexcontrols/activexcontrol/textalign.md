##ActiveXControl.TextAlign
ActiveXControl property. Represents how to align the text used by the control
## ActiveXControl.TextAlign property
Represents how to align the text used by the control.
```csharp
public TextAlignmentType TextAlign { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlPropertyTextAlignDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add two checkbox ActiveX controls
Shape shape1 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
Shape shape2 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 2, 0, 100, 30);
// Get the ActiveX controls
CheckBoxActiveXControl checkbox1 = (CheckBoxActiveXControl)shape1.ActiveXControl;
CheckBoxActiveXControl checkbox2 = (CheckBoxActiveXControl)shape2.ActiveXControl;
// Set different text alignments
checkbox1.TextAlign = TextAlignmentType.Center;
checkbox2.TextAlign = TextAlignmentType.Right;
// Display the text alignment values
Console.WriteLine("Checkbox1 TextAlign: " + checkbox1.TextAlign);
Console.WriteLine("Checkbox2 TextAlign: " + checkbox2.TextAlign);
}
}
}
```
### See Also
* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
