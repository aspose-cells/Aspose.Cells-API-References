##ListBoxActiveXControl.BorderOleColor
ListBoxActiveXControl property. Gets and sets the ole color of the background
## ListBoxActiveXControl.BorderOleColor property
Gets and sets the ole color of the background.
```csharp
public int BorderOleColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ListBoxActiveXControlPropertyBorderOleColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 0, 0, 200, 100);
ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
listBox.BorderOleColor = -2147483642;
workbook.Save("ListBoxBorderOleColorDemo.xlsm", SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
