##ListBox.SelectionType
ListBox property. Gets or sets the selection mode of the specified list box
## ListBox.SelectionType property
Gets or sets the selection mode of the specified list box.
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
public class ListBoxPropertySelectionTypeDemo
{
public static void Run()
{
// Create a new Workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the list box
sheet.Cells["A1"].PutValue("Sales");
sheet.Cells["A2"].PutValue("Finance");
sheet.Cells["A3"].PutValue("MIS");
sheet.Cells["A4"].PutValue("R&D");
// Add a list box
ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
// Set list box properties
listBox.InputRange = "A1:A4";
listBox.LinkedCell = "B1";
// Demonstrate SelectionType property
listBox.SelectionType = SelectionType.Single; // Only single selection allowed
listBox.SelectedIndex = 1; // Select "Finance"
// Save the workbook
workbook.Save("ListBoxSelectionTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
