##ActiveXControlBase.MouseIcon
ActiveXControlBase property. Gets and sets a custom icon to display as the mouse pointer for the control
## ActiveXControlBase.MouseIcon property
Gets and sets a custom icon to display as the mouse pointer for the control.
```csharp
public byte[] MouseIcon { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System.IO;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyMouseIconDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 0, 1, 0, 100, 100);
ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
imageControl.MouseIcon = File.ReadAllBytes("mouse.ico");
imageControl.MousePointer = ControlMousePointerType.Custom;
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
