##ListBoxActiveXControl.BorderStyle
ListBoxActiveXControl property. Gets and set the type of border used by the control
## ListBoxActiveXControl.BorderStyle property
Gets and set the type of border used by the control.
```csharp
public ControlBorderType BorderStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyBorderStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add ListBox ActiveX Control with corrected parameters
Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,
1, 0, 1, 100, 150, 30); // Added height parameter
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
// Set BorderStyle property
listBox.BorderStyle = ControlBorderType.None;
// Verify and output border style
Console.WriteLine("BorderStyle: " + listBox.BorderStyle);
workbook.Save("ListBoxBorderStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlBorderType](../../controlbordertype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
