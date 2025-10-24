##ActiveXControlBase.IsVisible
ActiveXControlBase property. Indicates whether this control is visible
## ActiveXControlBase.IsVisible property
Indicates whether this control is visible.
```csharp
public virtual bool IsVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyIsVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ListBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
var listBox = shape.ActiveXControl;
// Configure basic properties
listBox.IsVisible = true; // Demonstrate IsVisible property
Console.WriteLine("Initial visibility: " + listBox.IsVisible);
listBox.IsVisible = false;
Console.WriteLine("After setting to false: " + listBox.IsVisible);
listBox.IsVisible = true;
Console.WriteLine("After setting to true: " + listBox.IsVisible);
// Save the workbook
workbook.Save("ActiveXControlVisibilityDemo.xlsx");
}
}
}
```
### See Also
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
