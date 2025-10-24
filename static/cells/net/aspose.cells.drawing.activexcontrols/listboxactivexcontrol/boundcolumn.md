##ListBoxActiveXControl.BoundColumn
ListBoxActiveXControl property. Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value fmMultiSelectSingle
## ListBoxActiveXControl.BoundColumn property
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
public class ListBoxActiveXControlPropertyBoundColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B4"].PutValue("Banana");
// Add ListBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 150, 100);
Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;
// Configure ListBox properties
listBox.ColumnCount = 2;
listBox.ListFillRange = "A1:B4";
// Set BoundColumn to 0 (ID column) - this will be the value returned when an item is selected
listBox.BoundColumn = 0;
// Set TextColumn to 1 (Name column) - this will be displayed in the list
listBox.TextColumn = 1;
// Save the workbook
workbook.Save("ListBoxBoundColumnDemo.xlsx");
Console.WriteLine("ListBox BoundColumn set to: " + listBox.BoundColumn);
}
}
}
```
### See Also
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
