##ListBoxActiveXControl.MatchEntry
ListBoxActiveXControl property. Indicates how a ListBox or ComboBox searches its list as the user types
## ListBoxActiveXControl.MatchEntry property
Indicates how a ListBox or ComboBox searches its list as the user types.
```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyMatchEntryDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruits");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Cherry");
worksheet.Cells["A5"].PutValue("Date");
// Add ListBox ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 1, 0, 100, 80);
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
// Configure ListBox properties
listBox.ListWidth = 100;
listBox.ColumnCount = 1;
listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
listBox.Value = "Apple;Banana;Cherry;Date";
// Save the workbook
workbook.Save("ListBoxMatchEntryDemo.xlsx");
Console.WriteLine("ListBox with FirstLetter MatchEntry created successfully.");
}
}
}
```
### See Also
* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
