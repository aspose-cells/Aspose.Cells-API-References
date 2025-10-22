##Enum ControlScrollBarType
Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType enum. Represents the type of scroll bar
## ControlScrollBarType enumeration
Represents the type of scroll bar.
```csharp
public enum ControlScrollBarType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Displays no scroll bars. |
| Horizontal | `1` | Displays a horizontal scroll bar. |
| BarsVertical | `2` | Displays a vertical scroll bar. |
| BarsBoth | `3` | Displays both a horizontal and a vertical scroll bar. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ControlScrollBarTypeDemo
{
public static void ControlScrollBarTypeExample()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ListBox ActiveX control to the worksheet
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;
// Set the ScrollBars property to display both horizontal and vertical scroll bars
listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;
// Save the workbook
workbook.Save("ControlScrollBarTypeExample.xlsx");
workbook.Save("ControlScrollBarTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
