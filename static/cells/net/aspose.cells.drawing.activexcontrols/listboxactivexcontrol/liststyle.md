##ListBoxActiveXControl.ListStyle
ListBoxActiveXControl property. Gets and sets the visual appearance
## ListBoxActiveXControl.ListStyle property
Gets and sets the visual appearance.
```csharp
public ControlListStyle ListStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyListStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the list box
sheet.Cells["A3"].Value = "Sales";
sheet.Cells["A4"].Value = "Finance";
sheet.Cells["A5"].Value = "MIS";
sheet.Cells["A6"].Value = "R&D";
sheet.Cells["A7"].Value = "Marketing";
// Add a ListBox ActiveX control
Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
// Configure the ListBox properties
listBox.ListFillRange = "A3:A7";
listBox.LinkedCell = "B1";
listBox.ListStyle = ControlListStyle.Option; // Demonstrating ListStyle property
listBox.SelectionType = SelectionType.Single;
// Save the workbook
workbook.Save("ListBoxActiveXControl_ListStyle_Demo.xlsx");
}
}
}
```
### See Also
* enum [ControlListStyle](../../controlliststyle/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
