##ComboBoxActiveXControl.IsEditable
ComboBoxActiveXControl property. Indicates whether the user can type into the control
## ComboBoxActiveXControl.IsEditable property
Indicates whether the user can type into the control.
```csharp
public bool IsEditable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyIsEditableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control using Shapes collection
Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 5, 0, 100, 30);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ComboBox
comboBox.IsEditable = true;
comboBox.Value = "Editable ComboBox";
comboBox.ColumnCount = 2;
comboBox.ListRows = 6;
comboBox.TextColumn = 1;
// Add items to the ComboBox (using the ListFillRange property)
sheet.Cells["A10"].PutValue("Item 1");
sheet.Cells["B10"].PutValue("Description 1");
sheet.Cells["A11"].PutValue("Item 2");
sheet.Cells["B11"].PutValue("Description 2");
comboBox.ListFillRange = "A10:B11";
// Save the workbook
workbook.Save("ComboBoxActiveXControl_IsEditableDemo.xlsx");
// Verify property after save
Console.WriteLine("IsEditable property value: " + comboBox.IsEditable);
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
