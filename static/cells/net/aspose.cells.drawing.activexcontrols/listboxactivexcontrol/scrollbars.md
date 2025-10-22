##ListBoxActiveXControl.ScrollBars
ListBoxActiveXControl property. Indicates specifies whether the control has vertical scroll bars horizontal scroll bars both or neither
## ListBoxActiveXControl.ScrollBars property
Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither.
```csharp
public ControlScrollBarType ScrollBars { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyScrollBarsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 50);
Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBoxControl = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;
// Add some items to make scrollbars visible
listBoxControl.ListFillRange = "A1:A20";
for (int i = 1; i <= 20; i++)
{
worksheet.Cells["A" + i].PutValue("Item " + i);
}
// Demonstrate ScrollBars property
listBoxControl.ScrollBars = Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType.BarsBoth;
workbook.Save("ListBoxScrollBarsDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
