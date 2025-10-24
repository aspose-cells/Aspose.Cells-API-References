##ListBoxActiveXControl.ColumnCount
ListBoxActiveXControl property. Represents the number of columns to display in a ComboBox or ListBox
## ListBoxActiveXControl.ColumnCount property
Represents the number of columns to display in a ComboBox or ListBox.
```csharp
public int ColumnCount { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyColumnCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ListBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 1, 1, 1, 200, 100);
var listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;
// Set properties including ColumnCount
listBox.ColumnCount = 3;
listBox.ListFillRange = "A1:C3"; // Sample data range for 3 columns
// Verify and output the ColumnCount
Console.WriteLine("ListBox ColumnCount: " + listBox.ColumnCount);
// Save the workbook
workbook.Save("ListBoxActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
