##ActiveXControlBase.Height
ActiveXControlBase property. Gets and sets the height of the control in unit of points
## ActiveXControlBase.Height property
Gets and sets the height of the control in unit of points.
```csharp
public virtual double Height { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyHeightDemo
{
public static void Run()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
// Add a RadioButton ActiveXControl
Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;
// Set basic properties
activeXControl.Caption = "Height Demo";
activeXControl.IsAutoSize = false; // Disable auto-size to demonstrate Height property
// Demonstrate Height property
Console.WriteLine("Original Height: " + activeXControl.Height);
activeXControl.Height = 75;
Console.WriteLine("Modified Height: " + activeXControl.Height);
// Save the workbook
workbook.Save("ActiveXControlHeightDemo.xlsx");
}
}
}
```
### See Also
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
