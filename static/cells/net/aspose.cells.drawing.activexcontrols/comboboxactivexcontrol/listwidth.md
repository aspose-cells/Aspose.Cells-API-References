##ComboBoxActiveXControl.ListWidth
ComboBoxActiveXControl property. Gets and set the width in unit of points
## ComboBoxActiveXControl.ListWidth property
Gets and set the width in unit of points.
```csharp
public double ListWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertyListWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the ComboBox
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Orange");
// Add a ComboBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
1,  // left
1,  // top
100, // width
30,  // height
0,   // image width (unused for ComboBox)
0    // image height (unused for ComboBox)
);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox =
(Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Set ListWidth property to control dropdown width
comboBox.ListWidth = 150;
comboBox.ListRows = 3;
comboBox.LinkedCell = "A1:A3";
// Save the workbook
workbook.Save("ComboBoxListWidthDemo.xlsx");
Console.WriteLine("ComboBox ListWidth set to: " + comboBox.ListWidth);
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
