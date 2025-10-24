##ShapeCollection.UpdateSelectedValue
ShapeCollection method. Update the selected value by the value of the linked cell or range of the shape
## ShapeCollection.UpdateSelectedValue method
Update the selected value by the value of the linked cell or range of the shape.
```csharp
public void UpdateSelectedValue()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodUpdateSelectedValueDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape (dropdown list) to the worksheet
Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
// Set list items and selected value
listBox.SetInputRange("A1:A3", false, false);
listBox.SelectedIndex = 1;
// Update the selected value in the shape
worksheet.Shapes.UpdateSelectedValue();
// Save the workbook
workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
