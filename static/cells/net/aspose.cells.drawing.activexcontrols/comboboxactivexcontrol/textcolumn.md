##ComboBoxActiveXControl.TextColumn
ComboBoxActiveXControl property. Represents the column in a ComboBox or ListBox to display to the user
## ComboBoxActiveXControl.TextColumn property
Represents the column in a ComboBox or ListBox to display to the user.
```csharp
public int TextColumn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyTextColumnDemo
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
// Set up combo box properties
comboBox.ColumnCount = 2;
comboBox.ListRows = 5;
// Add items using ListFillRange (alternative to AddItem)
worksheet.Cells["A1"].PutValue("Item1");
worksheet.Cells["B1"].PutValue("Description1");
worksheet.Cells["A2"].PutValue("Item2");
worksheet.Cells["B2"].PutValue("Description2");
worksheet.Cells["A3"].PutValue("Item3");
worksheet.Cells["B3"].PutValue("Description3");
comboBox.ListFillRange = "A1:B3";
// Demonstrate TextColumn property
comboBox.TextColumn = 2; // Display second column (descriptions) as text
comboBox.BoundColumn = 1; // But bind to first column (items)
// Save the workbook
workbook.Save("ComboBoxTextColumnDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
