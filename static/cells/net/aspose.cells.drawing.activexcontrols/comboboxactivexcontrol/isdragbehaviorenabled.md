##ComboBoxActiveXControl.IsDragBehaviorEnabled
ComboBoxActiveXControl property. Indicates whether dragging and dropping is enabled for the control
## ComboBoxActiveXControl.IsDragBehaviorEnabled property
Indicates whether dragging and dropping is enabled for the control.
```csharp
public bool IsDragBehaviorEnabled { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyIsDragBehaviorEnabledDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 50);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox =
(Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Set some basic properties
comboBox.ListRows = 8;
comboBox.ColumnCount = 1;
comboBox.BoundColumn = 1;
comboBox.TextColumn = -1;
// Demonstrate IsDragBehaviorEnabled property
Console.WriteLine("Initial IsDragBehaviorEnabled: " + comboBox.IsDragBehaviorEnabled);
// Disable drag behavior
comboBox.IsDragBehaviorEnabled = false;
Console.WriteLine("After setting to false: " + comboBox.IsDragBehaviorEnabled);
// Enable drag behavior
comboBox.IsDragBehaviorEnabled = true;
Console.WriteLine("After setting to true: " + comboBox.IsDragBehaviorEnabled);
// Save the workbook
workbook.Save("ComboBoxActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
