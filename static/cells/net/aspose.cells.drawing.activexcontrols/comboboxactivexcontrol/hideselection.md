##ComboBoxActiveXControl.HideSelection
ComboBoxActiveXControl property. Indicates whether selected text in the control appears highlighted when the control does not have focus
## ComboBoxActiveXControl.HideSelection property
Indicates whether selected text in the control appears highlighted when the control does not have focus.
```csharp
public bool HideSelection { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyHideSelectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
10, 10, 150, 30, 100, 20);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox =
(Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Configure basic properties
comboBox.ListRows = 5;
comboBox.Value = "Select an item";
// Add sample items using the correct property name
comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
// Demonstrate HideSelection property
comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus
// Save the workbook
workbook.Save("ComboBoxHideSelectionDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
