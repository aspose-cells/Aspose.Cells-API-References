##ArcShape.EndArrowheadWidth
ArcShape property. Gets and sets the end arrow head width of the line
## ArcShape.EndArrowheadWidth property
Gets and sets the end arrow head width of the line.
```csharp
[Obsolete("Use Shape.Line.EndArrowheadWidth property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line.EndArrowheadWidth property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ArcShapePropertyEndArrowheadWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an Arc shape
ArcShape arc = worksheet.Shapes.AddArc(2, 0, 2, 0, 100, 100);
// Set line properties with arrowheads
arc.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
arc.EndArrowheadWidth = MsoArrowheadWidth.Medium;
// Display the current EndArrowheadWidth value
Console.WriteLine("End Arrowhead Width: " + arc.EndArrowheadWidth);
// Change the EndArrowheadWidth
arc.EndArrowheadWidth = MsoArrowheadWidth.Wide;
Console.WriteLine("Modified End Arrowhead Width: " + arc.EndArrowheadWidth);
// Save the workbook
workbook.Save("ArcShapeEndArrowheadWidthDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [ArcShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
