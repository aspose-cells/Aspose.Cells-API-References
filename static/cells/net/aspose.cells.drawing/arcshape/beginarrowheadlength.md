##ArcShape.BeginArrowheadLength
ArcShape property. Gets and sets the begin arrow head length of the line
## ArcShape.BeginArrowheadLength property
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
public class ArcShapePropertyBeginArrowheadLengthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an arc shape
ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);
// Set arrowhead properties
arc.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
arc.BeginArrowheadLength = MsoArrowheadLength.Medium;
arc.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
// Display the arrowhead length
Console.WriteLine("Begin Arrowhead Length: " + arc.BeginArrowheadLength);
// Modify the arrowhead length
arc.BeginArrowheadLength = MsoArrowheadLength.Long;
Console.WriteLine("Modified Begin Arrowhead Length: " + arc.BeginArrowheadLength);
// Save the workbook
workbook.Save("ArcShapeArrowheadDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [ArcShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
