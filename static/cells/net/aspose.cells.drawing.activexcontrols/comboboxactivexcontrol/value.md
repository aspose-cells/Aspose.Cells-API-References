##ComboBoxActiveXControl.Value
ComboBoxActiveXControl property. Gets and sets the value of the control
## ComboBoxActiveXControl.Value property
Gets and sets the value of the control.
```csharp
public string Value { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control to the worksheet
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 1, 0, 0, 100, 20);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ComboBox
comboBox.Value = "Initial Value";
comboBox.ListFillRange = "A1:A3";
// Add some sample data to the list range
worksheet.Cells["A1"].PutValue("Option 1");
worksheet.Cells["A2"].PutValue("Option 2");
worksheet.Cells["A3"].PutValue("Option 3");
// Update the selected value from linked cell
worksheet.Cells["B1"].PutValue("Option 2");
worksheet.Shapes.UpdateSelectedValue();
// Demonstrate getting the Value property
Console.WriteLine("ComboBox Value: " + comboBox.Value);
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
