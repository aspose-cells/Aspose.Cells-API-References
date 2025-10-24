##ListBoxActiveXControl.ShowColumnHeads
ListBoxActiveXControl property. Indicates whether column headings are displayed
## ListBoxActiveXControl.ShowColumnHeads property
Indicates whether column headings are displayed.
```csharp
public bool ShowColumnHeads { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyShowColumnHeadsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ListBox ActiveX Control with all required parameters
Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.ListBox,
1, 1, 100, 100,  // Left, Top, Width, Height
0, 0);           // UpperLeftRow, UpperLeftColumn
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ListBox
listBox.ColumnCount = 2;
listBox.ListWidth = 150;
listBox.ShowColumnHeads = true; // Demonstrate ShowColumnHeads property
// Add some sample data
listBox.Value = "Header1\tHeader2\nItem1\tData1\nItem2\tData2";
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
