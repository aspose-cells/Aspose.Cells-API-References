##Enum ControlListStyle
Aspose.Cells.Drawing.ActiveXControls.ControlListStyle enum. Represents the visual appearance of the list in a ListBox or ComboBox
## ControlListStyle enumeration
Represents the visual appearance of the list in a ListBox or ComboBox.
```csharp
public enum ControlListStyle
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Plain | `0` | Displays a list in which the background of an item is highlighted when it is selected. |
| Option | `1` | Displays a list in which an option button or a checkbox next to each entry displays the selection state of that item. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ControlListStyleDemo
{
public static void ControlListStyleExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Item 1");
worksheet.Cells["A3"].PutValue("Item 2");
worksheet.Cells["A4"].PutValue("Item 3");
// Add a ComboBox ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ComboBox
comboBox.ListWidth = 100;
comboBox.ListRows = 3;
comboBox.ColumnCount = 1;
comboBox.ListStyle = ControlListStyle.Plain; // Set the ListStyle to Plain
// Add items to the ComboBox
comboBox.Value = "Item 1";
comboBox.BoundColumn = 1;
comboBox.TextColumn = 1;
// Add a ListBox ActiveX control to the worksheet
var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;
// Set properties for the ListBox
listBox.ColumnCount = 1;
listBox.ListStyle = ControlListStyle.Option; // Set the ListStyle to Option
// Add items to the ListBox
listBox.Value = "Item 1";
listBox.BoundColumn = 1;
listBox.TextColumn = 1;
// Save the workbook
workbook.Save("ControlListStyleExample.xlsx");
workbook.Save("ControlListStyleExample.pdf");
// Output the results
Console.WriteLine("ComboBox ListStyle: " + comboBox.ListStyle);
Console.WriteLine("ListBox ListStyle: " + listBox.ListStyle);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
