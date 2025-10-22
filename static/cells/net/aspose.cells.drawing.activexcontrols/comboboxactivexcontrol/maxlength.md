##ComboBoxActiveXControl.MaxLength
ComboBoxActiveXControl property. Gets and sets the maximum number of characters
## ComboBoxActiveXControl.MaxLength property
Gets and sets the maximum number of characters
```csharp
public int MaxLength { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyMaxLengthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
5, 0, 100, 20, 100, 20);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox =
(Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Set MaxLength property and other essential properties
comboBox.MaxLength = 10; // Restrict input to 10 characters
comboBox.ListRows = 5;
comboBox.IsEditable = true;
comboBox.Value = "Test";
// Save the workbook
workbook.Save("ComboBoxMaxLengthDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
