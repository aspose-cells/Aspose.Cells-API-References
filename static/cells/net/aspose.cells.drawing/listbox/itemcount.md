##ListBox.ItemCount
ListBox property. Gets the number of items in the list box
## ListBox.ItemCount property
Gets the number of items in the list box.
```csharp
public int ItemCount { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ListBoxPropertyItemCountDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets.Add("Sheet1");
// Add sample data
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Mango");
// Create list box and set properties
Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 10, 0, 100, 150);
listBox.InputRange = "A1:A4";
// Demonstrate ItemCount usage
int itemCount = listBox.ItemCount;
Console.WriteLine("ListBox contains {0} items", itemCount);
// Adjust listbox height based on item count
listBox.Height = itemCount * 15;
workbook.Save("ListBoxItemCountDemo.xlsx");
}
}
}
```
### See Also
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
