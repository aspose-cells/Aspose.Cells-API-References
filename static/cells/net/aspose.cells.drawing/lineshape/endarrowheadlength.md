##LineShape.EndArrowheadLength
LineShape property. Gets and sets the end arrow head length of the line
## LineShape.EndArrowheadLength property
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
public class LineShapePropertyEndArrowheadLengthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
LineShape line = worksheet.Shapes.AddLine(5, 0, 5, 5, 50, 150);
// Set line properties including end arrowhead length
line.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
line.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
line.EndArrowheadLength = MsoArrowheadLength.Long;
// Save the workbook
workbook.Save("LineShapeEndArrowheadLengthDemo.xlsx");
// Display the end arrowhead length
Console.WriteLine("End Arrowhead Length: " + line.EndArrowheadLength);
}
}
}
```
### See Also
* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
