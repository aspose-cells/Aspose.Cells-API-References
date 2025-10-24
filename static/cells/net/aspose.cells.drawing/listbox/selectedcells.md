##ListBox.SelectedCells
ListBox property. Gets the selected cells. Returns null if the input range is not set or no item is selected
## ListBox.SelectedCells property
Gets the selected cells. Returns null if the input range is not set or no item is selected
```csharp
public Cell[] SelectedCells { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ListBoxPropertySelectedCellsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data for ListBox items
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
worksheet.Cells["A4"].PutValue("Item 4");
worksheet.Cells["A5"].PutValue("Item 5");
// Create a ListBox and bind it to the data range
ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
listBox.InputRange = "A1:A5";
listBox.SelectionType = SelectionType.Multi;
// Select multiple items using zero-based indexes
listBox.SelectedItem(0, true);
listBox.SelectedItem(2, true);
// Retrieve and display selected cells
Cell[] selectedCells = listBox.SelectedCells;
Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
// Modify selected cells to demonstrate access
foreach (Cell cell in selectedCells)
{
Console.WriteLine("Selected Cell Address: " + cell.Name);
cell.PutValue("[SELECTED] " + cell.StringValue);
}
workbook.Save("ListBoxSelectedCellsDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
