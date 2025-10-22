##ActiveXControlBase.LinkedCell
ActiveXControlBase property. Gets and sets the linked cell
## ActiveXControlBase.LinkedCell property
Gets and sets the linked cell.
```csharp
public string LinkedCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyLinkedCellDemo
{
public static void Run()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
// Add a SpinButtonActiveXControl to the first worksheet
Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
10, 10, 100, 30, 100, 30);
Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton =
(Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
// Configure the spin button properties
spinButton.Min = 0;
spinButton.Max = 100;
spinButton.Position = 50;
spinButton.SmallChange = 1;
// Link the control to cell A1
spinButton.LinkedCell = "A1";
// Set cell A1's value to match the initial position
workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);
// Save the workbook
workbook.Save("LinkedCellDemo.xlsx");
}
}
}
```
### See Also
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
