##UnknownControl.Type
UnknownControl property. Gets the type of the ActiveX control
## UnknownControl.Type property
Gets the type of the ActiveX control.
```csharp
public override ControlType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class UnknownControlPropertyTypeDemo
{
public static void Run()
{
// Load existing workbook containing unknown control
Workbook workbook = new Workbook("input_with_unknown_control.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
// Find and process UnknownControl instances
foreach (Shape shape in worksheet.Shapes)
{
if (shape.ActiveXControl is UnknownControl control)
{
// Demonstrate reading Type property
Console.WriteLine($"Found control with Type: {control.Type}");
// Example usage based on control type
if (control.Type == ControlType.ListBox)
{
Console.WriteLine("Processing legacy ListBox control");
}
else if (control.Type == ControlType.Unknown)
{
Console.WriteLine("Handling completely unknown control type");
}
}
}
// Save processed workbook
workbook.Save("ControlTypeAnalysis.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
