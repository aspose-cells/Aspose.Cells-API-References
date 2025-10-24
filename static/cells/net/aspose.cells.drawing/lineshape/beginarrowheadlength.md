##LineShape.BeginArrowheadLength
LineShape property. Gets and sets the begin arrow head length of the line
## LineShape.BeginArrowheadLength property
Gets and sets the begin arrow head length of the line.
```csharp
[Obsolete("Use Shape.Line.BeginArrowheadLength property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line.BeginArrowheadLength property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineShapePropertyBeginArrowheadLengthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);
// Set arrowhead properties
line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
line.BeginArrowheadLength = MsoArrowheadLength.Medium;
line.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
// Display the set arrowhead length
Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowheadLength);
// Save the workbook
workbook.Save("LineShapeArrowheadDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
