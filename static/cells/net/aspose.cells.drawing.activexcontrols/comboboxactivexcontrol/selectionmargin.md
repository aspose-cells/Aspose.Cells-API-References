##ComboBoxActiveXControl.SelectionMargin
ComboBoxActiveXControl property. Indicates whether the user can select a line of text by clicking in the region to the left of the text
## ComboBoxActiveXControl.SelectionMargin property
Indicates whether the user can select a line of text by clicking in the region to the left of the text.
```csharp
public bool SelectionMargin { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxActiveXControlPropertySelectionMarginDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;
// Demonstrate SelectionMargin property
comboBox.SelectionMargin = false;
Console.WriteLine("SelectionMargin set to: " + comboBox.SelectionMargin);
// Toggle and demonstrate again
comboBox.SelectionMargin = true;
Console.WriteLine("SelectionMargin now set to: " + comboBox.SelectionMargin);
workbook.Save("ComboBoxSelectionMarginDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
