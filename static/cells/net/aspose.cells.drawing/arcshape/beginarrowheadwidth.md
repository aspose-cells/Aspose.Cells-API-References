##ArcShape.BeginArrowheadWidth
ArcShape property. Gets and sets the begin arrow head width of the line
## ArcShape.BeginArrowheadWidth property
Gets and sets the begin arrow head width of the line.
```csharp
[Obsolete("Use Shape.Line.BeginArrowheadWidth property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line.BeginArrowheadWidth property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ArcShapePropertyBeginArrowheadWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an arc shape
ArcShape arc = worksheet.Shapes.AddArc(2, 0, 2, 0, 100, 100);
// Set arrowhead properties
arc.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
arc.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
// Display the arrowhead width
Console.WriteLine("Begin Arrowhead Width: " + arc.BeginArrowheadWidth);
// Modify the arrowhead width
arc.BeginArrowheadWidth = MsoArrowheadWidth.Wide;
Console.WriteLine("Modified Begin Arrowhead Width: " + arc.BeginArrowheadWidth);
// Save the workbook
workbook.Save("ArcShapeArrowheadDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [ArcShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
