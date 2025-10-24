##Enum SelectionType
Aspose.Cells.Drawing.SelectionType enum. The selection type of list box
## SelectionType enumeration
The selection type of list box.
```csharp
public enum SelectionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Single | `0` | Sigle selection type. |
| Multi | `1` | Multiple selection type. |
| Extend | `2` | Extend selection type. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassSelectionTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a list box to the worksheet
ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);
// Set the selection type to Single
listBox.SelectionType = SelectionType.Single;
// Add items to the list box
listBox.SetInputRange("A1:A5", false, false);
// Verify the selection type
Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);
// Save the workbook
workbook.Save("SelectionTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
