##ComboBoxActiveXControl.ColumnCount
ComboBoxActiveXControl property. Represents the number of columns to display in a ComboBox or ListBox
## ComboBoxActiveXControl.ColumnCount property
Represents the number of columns to display in a ComboBox or ListBox.
```csharp
public int ColumnCount { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyColumnCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruits");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Cherry");
// Add ComboBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Set ColumnCount property and other properties
comboBox.ColumnCount = 1;
comboBox.ListWidth = 100;
comboBox.Value = "Apple;Banana;Cherry";
// Save the workbook
workbook.Save("ComboBoxColumnCountDemo.xlsx");
Console.WriteLine("ComboBox with ColumnCount=1 has been created and saved.");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
