##ComboBoxActiveXControl.ShowColumnHeads
ComboBoxActiveXControl property. Indicates whether column headings are displayed
## ComboBoxActiveXControl.ShowColumnHeads property
Indicates whether column headings are displayed.
```csharp
public bool ShowColumnHeads { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyShowColumnHeadsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox =
(Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ComboBox
comboBox.ColumnCount = 2;
comboBox.ListWidth = 100;
// Add sample data to the ComboBox
comboBox.ListFillRange = "A1:B3";
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue("Value1");
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B3"].PutValue("Value2");
// Demonstrate ShowColumnHeads property
Console.WriteLine("Initial ShowColumnHeads value: " + comboBox.ShowColumnHeads);
// Enable column headers
comboBox.ShowColumnHeads = true;
Console.WriteLine("After setting ShowColumnHeads to true: " + comboBox.ShowColumnHeads);
// Disable column headers
comboBox.ShowColumnHeads = false;
Console.WriteLine("After setting ShowColumnHeads to false: " + comboBox.ShowColumnHeads);
// Save the workbook
workbook.Save("ComboBoxShowColumnHeadsDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
