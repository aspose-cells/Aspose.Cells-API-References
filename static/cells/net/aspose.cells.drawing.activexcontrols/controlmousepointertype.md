##Enum ControlMousePointerType
Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType enum. Represents the type of icon displayed as the mouse pointer for the control
## ControlMousePointerType enumeration
Represents the type of icon displayed as the mouse pointer for the control.
```csharp
public enum ControlMousePointerType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Standard pointer. |
| Arrow | `1` | Arrow. |
| Cross | `2` | Cross-hair pointer. |
| IBeam | `3` | I-beam. |
| SizeNESW | `6` | Double arrow pointing northeast and southwest. |
| SizeNS | `7` | Double arrow pointing north and south. |
| SizeNWSE | `8` | Double arrow pointing northwest and southeast. |
| SizeWE | `9` | Double arrow pointing west and east. |
| UpArrow | `10` | Up arrow. |
| HourGlass | `11` | Hourglass. |
| NoDrop | `12` | "Not” symbol (circle with a diagonal line) on top of the object being dragged. |
| AppStarting | `13` | Arrow with an hourglass. |
| Help | `14` | Arrow with a question mark. |
| SizeAll | `15` | "Size-all” cursor (arrows pointing north, south, east, and west). |
| Custom | `99` | Uses the icon specified by the MouseIcon property. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ControlMousePointerTypeDemo
{
public static void ControlMousePointerTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add an ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;
// Cast the ActiveXControl to ActiveXControlBase to access its properties
ActiveXControlBase controlBase = control as ActiveXControlBase;
if (controlBase != null)
{
// Set the mouse pointer type for the control
controlBase.MousePointer = ControlMousePointerType.Cross;
// Set other properties for demonstration
controlBase.Width = 150;
controlBase.Height = 50;
controlBase.IsVisible = true;
controlBase.Shadow = true;
controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
}
// Save the workbook
workbook.Save("ControlMousePointerTypeExample.xlsx");
workbook.Save("ControlMousePointerTypeExample.pdf");
// Output the result
Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
