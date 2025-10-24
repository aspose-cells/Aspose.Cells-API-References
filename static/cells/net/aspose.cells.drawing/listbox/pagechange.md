##ListBox.PageChange
ListBox property. Specifies the amount by which the controls value is changed when the user clicks on the scrollbars page up or page down region
## ListBox.PageChange property
Specifies the amount by which the control's value is changed when the user clicks on the scrollbar's page up or page down region.
```csharp
public int PageChange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListBoxPropertyPageChangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ListBox shape
ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);
// Set some items for the ListBox
listBox.SetInputRange("A1:A5", false, false);
// Set the PageChange property
listBox.PageChange = 2;
// Save the workbook
workbook.Save("ListBoxPageChangeDemo.xlsx");
// Display the PageChange value
Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
}
}
}
```
### See Also
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
