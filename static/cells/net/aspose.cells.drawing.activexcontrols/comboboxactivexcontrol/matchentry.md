##ComboBoxActiveXControl.MatchEntry
ComboBoxActiveXControl property. Indicates how a ListBox or ComboBox searches its list as the user types
## ComboBoxActiveXControl.MatchEntry property
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
public class ComboBoxActiveXControlPropertyMatchEntryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ComboBox ActiveX control to the worksheet
Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.ComboBox,
1, 0, 1, 0, 100, 20);
// Get the ComboBox ActiveX control
ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
// Configure basic properties
comboBox.Font.Name = "Arial";
comboBox.Font.Size = 10;
comboBox.ListRows = 8;
// Demonstrate MatchEntry property
comboBox.MatchEntry = ControlMatchEntryType.Complete; // Search as user types
Console.WriteLine("MatchEntry set to: " + comboBox.MatchEntry);
// Change MatchEntry to another mode
comboBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Search by first letter
Console.WriteLine("MatchEntry changed to: " + comboBox.MatchEntry);
// Save the workbook
workbook.Save("ComboBoxActiveXControlDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
