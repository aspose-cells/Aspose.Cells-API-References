##ListBox.SelectedItem
ListBox method. Sets whether the item is selected
## ListBox.SelectedItem method
Sets whether the item is selected
```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```
| Parameter | Type | Description |
| --- | --- | --- |
| itemIndex | Int32 | The item index |
| isSelected | Boolean | Whether the item is selected. True means that this item should be selected. False means that this item should be unselected. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ListBoxMethodSelectedItemWithInt32BooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate list items
for (int i = 0; i < 5; i++)
{
worksheet.Cells[i, 0].Value = $"Item {i + 1}";
}
// Create list box
ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
listBox.InputRange = "A1:A5";
listBox.SelectionType = SelectionType.Multi;
try
{
// Select and deselect items
listBox.SelectedItem(2, true);  // Select third item (index 2)
listBox.SelectedItem(0, true);   // Select first item (index 0)
listBox.SelectedItem(2, false); // Deselect third item
// Verify selections
Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");
// Display selected cells
Console.WriteLine("\nSelected Items:");
foreach (Cell cell in listBox.SelectedCells)
{
Console.WriteLine(cell.Value);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("ListBoxMethodSelectedItemWithInt32BooleanDemo.xlsx");
}
}
}
```
### See Also
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
