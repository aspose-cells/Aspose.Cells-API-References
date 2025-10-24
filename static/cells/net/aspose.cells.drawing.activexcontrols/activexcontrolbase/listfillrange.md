##ActiveXControlBase.ListFillRange
ActiveXControlBase property. Gets and sets the list fill range
## ActiveXControlBase.ListFillRange property
Gets and sets the list fill range.
```csharp
public string ListFillRange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyListFillRangeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for ListFillRange
for (int i = 1; i <= 10; i++)
{
worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
}
// Add a ComboBoxActiveXControl
Shape shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
1, 0, 100, 50, 100, 50);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox =
(Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Set ListFillRange to populate the combobox
comboBox.ListFillRange = "A2:A10";
// Save the workbook
workbook.Save("ActiveXControlListFillRangeDemo.xlsx");
}
}
}
```
### See Also
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
