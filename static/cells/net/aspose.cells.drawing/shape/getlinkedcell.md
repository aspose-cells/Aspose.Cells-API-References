##Shape.GetLinkedCell
Shape method. Gets the range linked to the controls value
## Shape.GetLinkedCell method
Gets the range linked to the control's value.
```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Return Value
The range linked to the control's value.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodGetLinkedCellWithBooleanBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set its linked cell
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
shape.LinkedCell = "A1";
// Get the linked cell address with different parameter combinations
string link1 = shape.GetLinkedCell(false, false); // Returns absolute reference like "$A$1"
string link2 = shape.GetLinkedCell(true, false);   // Returns relative reference like "A1"
string link3 = shape.GetLinkedCell(false, true);   // Returns R1C1 style absolute reference
Console.WriteLine("Linked cell (absolute A1): " + link1);
Console.WriteLine("Linked cell (relative A1): " + link2);
Console.WriteLine("Linked cell (R1C1 style): " + link3);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
