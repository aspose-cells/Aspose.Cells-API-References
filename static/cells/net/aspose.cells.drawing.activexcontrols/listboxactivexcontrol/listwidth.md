##ListBoxActiveXControl.ListWidth
ListBoxActiveXControl property. Gets and set the width in unit of points
## ListBoxActiveXControl.ListWidth property
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
public class ListBoxActiveXControlPropertyListWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add ListBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,
10, 10, 200, 100, 200, 100);
Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox =
(Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;
// Set ListWidth property
listBox.ListWidth = 150;
// Configure basic properties
listBox.ColumnCount = 2;
listBox.ColumnWidths = 100; // Changed from string to double
// Add sample data
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Red");
worksheet.Cells["B2"].PutValue("Yellow");
worksheet.Cells["B3"].PutValue("Orange");
// Set data range
listBox.ListFillRange = "A1:B3";
workbook.Save("ListBoxWidthDemo.xlsx");
Console.WriteLine("ListBox with ListWidth=150 created successfully.");
}
}
}
```
### See Also
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
