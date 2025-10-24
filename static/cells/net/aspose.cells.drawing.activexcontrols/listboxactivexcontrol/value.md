##ListBoxActiveXControl.Value
ListBoxActiveXControl property. Gets and sets the value of the control
## ListBoxActiveXControl.Value property
Gets and sets the value of the control.
```csharp
public string Value { get; set; }
```
### Remarks
Only effects when [`SelectionType`](../selectiontype/) is SelectionType.Single;
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ListBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 60);
Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;
// Set basic properties
listBox.ListWidth = 100;
listBox.ColumnCount = 1;
// Set items using Value property
listBox.Value = "Red;Green;Blue;Yellow";
// Save the workbook
workbook.Save("ListBoxValueDemo.xlsx");
Console.WriteLine("ListBox with items set using Value property has been created.");
}
}
}
```
### See Also
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
