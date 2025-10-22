##ListBoxActiveXControl.SelectionType
ListBoxActiveXControl property. Indicates whether the control permits multiple selections
## ListBoxActiveXControl.SelectionType property
Indicates whether the control permits multiple selections.
```csharp
public SelectionType SelectionType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertySelectionTypeDemo
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
// Add ListBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;
// Configure ListBox properties
listBox.ListWidth = 100;
listBox.ColumnCount = 1;
// Demonstrate SelectionType property
listBox.SelectionType = SelectionType.Single; // Only single selection allowed
listBox.Value = "Apple;Banana;Cherry";
// Save the workbook
workbook.Save("ListBoxSelectionTypeDemo.xlsx");
Console.WriteLine("ListBox with Single SelectionType created successfully.");
}
}
}
```
### See Also
* enum [SelectionType](../../../aspose.cells.drawing/selectiontype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
