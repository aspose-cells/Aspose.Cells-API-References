##ListBox.SelectedIndex
ListBox property. Gets or sets the index number of the currently selected item in a list box or combo box. Zerobased
## ListBox.SelectedIndex property
Gets or sets the index number of the currently selected item in a list box or combo box. Zero-based.
```csharp
public int SelectedIndex { get; set; }
```
### Remarks
-1 presents no item is selected.
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListBoxPropertySelectedIndexDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Item 0");
worksheet.Cells["A2"].PutValue("Item 1");
worksheet.Cells["A3"].PutValue("Item 2");
ListBox listBox = worksheet.Shapes.AddListBox(5, 5, 100, 100, 200, 300);
listBox.InputRange = "A1:A3";
listBox.LinkedCell = "B1";
listBox.SelectedIndex = 2;
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
