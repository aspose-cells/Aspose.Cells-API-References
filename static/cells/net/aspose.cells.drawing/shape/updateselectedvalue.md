##Shape.UpdateSelectedValue
Shape method. Update the selected value by the value of the linked cell
## Shape.UpdateSelectedValue method
Update the selected value by the value of the linked cell.
```csharp
public void UpdateSelectedValue()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodUpdateSelectedValueDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].Value = i + 1;
}
// Create a ListBox shape
Shape listBoxShape = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
// Set input range and linked cell
listBoxShape.SetInputRange("$A$1:$A$6", false, false);
listBoxShape.SetLinkedCell("$A$12", false, true);
// Get the ListBox object
ListBox listBox = (ListBox)listBoxShape;
// Set initial value in linked cell and update selection
worksheet.Cells["A12"].Value = 3;
listBoxShape.UpdateSelectedValue();
// Verify selection
if (listBox.IsSelected(2))
{
Console.WriteLine("Option 3 is selected");
}
// Change value and update selection again
worksheet.Cells["A12"].Value = 4;
listBoxShape.UpdateSelectedValue();
if (listBox.IsSelected(3))
{
Console.WriteLine("Option 4 is selected");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
