##ArcShape.EndArrowheadLength
ArcShape property. Gets and sets the end arrow head length of the line
## ArcShape.EndArrowheadLength property
Gets and sets the end arrow head length of the line.
```csharp
[Obsolete("Use Shape.Line.EndArrowheadLength property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadLength EndArrowheadLength { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line.EndArrowheadLength property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ArcShapePropertyEndArrowheadLengthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an Arc shape
ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);
// Set line properties with arrowheads
arc.LineFormat.IsVisible = true;
arc.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
arc.EndArrowheadLength = MsoArrowheadLength.Long; // Demonstrating EndArrowheadLength property
// Display the arrowhead length
Console.WriteLine("End Arrowhead Length: " + arc.EndArrowheadLength);
// Save the workbook
workbook.Save("ArcShapePropertyEndArrowheadLengthDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [ArcShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
