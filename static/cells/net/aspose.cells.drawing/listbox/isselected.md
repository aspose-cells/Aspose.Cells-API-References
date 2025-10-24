##ListBox.IsSelected
ListBox method. Indicates whether the item is selected
## ListBox.IsSelected method
Indicates whether the item is selected.
```csharp
public bool IsSelected(int itemIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| itemIndex | Int32 | The item index. |
### Return Value
whether the item is selected.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListBoxMethodIsSelectedWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a list box to the worksheet
ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);
// Set list items through the linked cell range
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
listBox.LinkedCell = "A1:A3";
// Select an item
listBox.SelectedIndex = 0;
// Check selection status using IsSelected with Int32 parameter
Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
}
}
}
```
### See Also
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
