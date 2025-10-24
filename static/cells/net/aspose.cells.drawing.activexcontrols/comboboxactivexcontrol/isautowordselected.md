##ComboBoxActiveXControl.IsAutoWordSelected
ComboBoxActiveXControl property. Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word
## ComboBoxActiveXControl.IsAutoWordSelected property
Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.
```csharp
public virtual bool IsAutoWordSelected { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyIsAutoWordSelectedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 100, 20, 100, 20);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Configure basic properties
comboBox.ListRows = 5;
comboBox.ColumnCount = 1;
comboBox.Value = "Sample Text";
// Demonstrate IsAutoWordSelected property
comboBox.IsAutoWordSelected = false;
Console.WriteLine("IsAutoWordSelected set to: " + comboBox.IsAutoWordSelected);
// Save the workbook
workbook.Save("ComboBoxIsAutoWordSelectedDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
