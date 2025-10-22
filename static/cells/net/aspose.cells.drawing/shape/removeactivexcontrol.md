##Shape.RemoveActiveXControl
Shape method. Remove activeX control
## Shape.RemoveActiveXControl method
Remove activeX control.
```csharp
public void RemoveActiveXControl()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodRemoveActiveXControlDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape that will contain the ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton,
1, 1, 1, 1, 100, 50);
// Remove the ActiveX control if it exists
if (shape.ActiveXControl != null)
{
shape.RemoveActiveXControl();
Console.WriteLine("ActiveX control removed successfully.");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
