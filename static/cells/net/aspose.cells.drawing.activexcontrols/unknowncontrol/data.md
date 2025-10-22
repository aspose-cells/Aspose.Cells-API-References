##UnknownControl.Data
UnknownControl property. Gets and sets the binary data of the control
## UnknownControl.Data property
Gets and sets the binary data of the control.
```csharp
public override byte[] Data { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class UnknownControlPropertyDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a dummy CLSID (invalid identifier)
byte[] dummyClsid = new byte[16];
// Add an unknown ActiveX control using ControlType.Unknown with full parameters
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);
// Access the UnknownControl instance
UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;
// Set the control's data including CLSID by copying into existing array
Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);
// Read and display Data property information
Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
Console.WriteLine($"Control type: {unknownControl.Type}");
// Demonstrate persistence of control data in output file
workbook.Save("UnknownControlDataDemo.xlsx");
}
}
}
```
### See Also
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
