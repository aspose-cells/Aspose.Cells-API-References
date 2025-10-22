##ShapeCollection.AddListBox
ShapeCollection method. Adds a ListBox to the worksheet
## ShapeCollection.AddListBox method
Adds a ListBox to the worksheet.
```csharp
public ListBox AddListBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height,
int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of ListBox from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of ListBox from its left column, in unit of pixel. |
| height | Int32 | Represents the height of ListBox, in unit of pixel. |
| width | Int32 | Represents the width of ListBox, in unit of pixel. |
### Return Value
A ListBox object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddListBoxWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a list box to the worksheet
Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 50);
// Add items to the list box
listBox.SetInputRange("A1:A3", false, false);
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
// Save the workbook
workbook.Save("ListBoxDemo.xlsx");
}
}
}
```
### See Also
* class [ListBox](../../listbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
