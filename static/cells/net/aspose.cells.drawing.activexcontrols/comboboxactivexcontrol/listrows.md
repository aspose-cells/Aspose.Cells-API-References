##ComboBoxActiveXControl.ListRows
ComboBoxActiveXControl property. Represents the maximum number of rows to display in the list
## ComboBoxActiveXControl.ListRows property
Represents the maximum number of rows to display in the list.
```csharp
public int ListRows { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyListRowsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control with proper width/height parameters
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 10, 10, 150, 30, 100, 20);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Add sample items to the combo box using ListFillRange
comboBox.ListFillRange = "A1:A7";
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
worksheet.Cells["A4"].PutValue("Item 4");
worksheet.Cells["A5"].PutValue("Item 5");
worksheet.Cells["A6"].PutValue("Item 6");
worksheet.Cells["A7"].PutValue("Item 7");
// Set ListRows property to control visible items in dropdown
comboBox.ListRows = 4; // Only show 4 items at a time
// Save the workbook
workbook.Save("ComboBoxListRowsDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
