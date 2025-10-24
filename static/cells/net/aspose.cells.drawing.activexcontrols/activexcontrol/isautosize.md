##ActiveXControl.IsAutoSize
ActiveXControl property. Indicates whether the control will automatically resize to display its entire contents
## ActiveXControl.IsAutoSize property
Indicates whether the control will automatically resize to display its entire contents.
```csharp
public virtual bool IsAutoSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlPropertyIsAutoSizeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Corrected AddActiveXControl parameters with full signature
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 0, 0, 100, 50);
ActiveXControl control = shape.ActiveXControl;
Console.WriteLine("Initial IsAutoSize: " + control.IsAutoSize);
control.IsAutoSize = true;
Console.WriteLine("Set IsAutoSize: " + control.IsAutoSize);
string outputPath = "AutoSizeControlDemo.xlsm";
workbook.Save(outputPath, SaveFormat.Xlsm);
Workbook loadedWorkbook = new Workbook(outputPath);
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
ActiveXControl loadedControl = loadedShape.ActiveXControl;
Console.WriteLine("Loaded IsAutoSize: " + loadedControl.IsAutoSize);
}
}
}
```
### See Also
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
