##Shape.ControlData
Shape property. Gets the data of control
## Shape.ControlData property
Gets the data of control.
```csharp
public byte[] ControlData { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyControlDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Access ControlData (read-only property)
byte[] controlData = shape.ControlData;
// Check ControlData
if (controlData != null)
{
Console.WriteLine("ControlData exists with length: " + controlData.Length);
}
else
{
Console.WriteLine("No data.");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
