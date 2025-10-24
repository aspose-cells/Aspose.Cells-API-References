##ComboBoxActiveXControl.BoundColumn
ComboBoxActiveXControl property. Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value fmMultiSelectSingle
## ComboBoxActiveXControl.BoundColumn property
Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle).
```csharp
public int BoundColumn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyBoundColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B4"].PutValue("Banana");
// Add a ComboBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 150, 20);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Configure the ComboBox
comboBox.ListFillRange = "A1:B4";
comboBox.ColumnCount = 2;
comboBox.BoundColumn = 0; // Bind to the ID column (column index 0)
comboBox.TextColumn = 1; // Display the Name column (column index 1)
// Save the workbook
workbook.Save("ComboBoxBoundColumnDemo.xlsx");
Console.WriteLine("ComboBox BoundColumn set to: " + comboBox.BoundColumn);
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
