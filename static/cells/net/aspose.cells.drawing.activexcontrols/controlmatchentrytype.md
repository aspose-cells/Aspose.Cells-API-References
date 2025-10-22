##Enum ControlMatchEntryType
Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType enum. Represents how a ListBox or ComboBox searches its list as the user types
## ControlMatchEntryType enumeration
Represents how a ListBox or ComboBox searches its list as the user types.
```csharp
public enum ControlMatchEntryType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| FirstLetter | `0` | The control searches for the next entry that starts with the character entered. Repeatedly typing the same letter cycles through all entries beginning with that letter. |
| Complete | `1` | As each character is typed, the control searches for an entry matching all characters entered. |
| None | `2` | The list will not be searched when characters are typed. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ControlMatchEntryTypeDemo
{
public static void ControlMatchEntryTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Cherry");
// Add a ComboBox ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Set properties for the ComboBox
comboBox.ListWidth = 100;
comboBox.ListRows = 3;
comboBox.ColumnCount = 1;
comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
comboBox.IsEditable = true;
// Add items to the ComboBox
comboBox.Value = "Apple;Banana;Cherry";
// Add a ListBox ActiveX control to the worksheet
var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;
// Set properties for the ListBox
listBox.ListWidth = 100;
listBox.ColumnCount = 1;
listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
listBox.SelectionType = SelectionType.Single;
// Add items to the ListBox
listBox.Value = "Apple;Banana;Cherry";
// Save the workbook
workbook.Save("ControlMatchEntryTypeExample.xlsx");
workbook.Save("ControlMatchEntryTypeExample.pdf");
// Output the results
Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
