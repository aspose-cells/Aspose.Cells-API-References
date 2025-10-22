##ListBoxActiveXControl.Type
ListBoxActiveXControl property. Gets the type of the ActiveX control
## ListBoxActiveXControl.Type property
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
public class ListBoxActiveXControlPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a ListBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 0, 0);
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
// Demonstrate the Type property
Console.WriteLine("Control Type: " + listBox.Type);
// Set some properties
listBox.ScrollBars = ControlScrollBarType.BarsBoth;
listBox.ColumnCount = 1;
listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
listBox.ListStyle = ControlListStyle.Plain;
listBox.SelectionType = SelectionType.Single;
// Verify the Type property
if (listBox.Type == ControlType.ListBox)
{
Console.WriteLine("This is a ListBox control as expected");
}
// Save the workbook
workbook.Save("ListBoxActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
