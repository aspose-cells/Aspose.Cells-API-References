##LineShape.BeginArrowheadWidth
LineShape property. Gets and sets the begin arrow head width of the line
## LineShape.BeginArrowheadWidth property
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
public class LineShapePropertyBeginArrowheadWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);
// Set line properties including BeginArrowheadWidth
line.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
line.EndArrowheadWidth = MsoArrowheadWidth.Narrow;
// Display the set values
Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowheadWidth);
Console.WriteLine("End Arrowhead Width: " + line.EndArrowheadWidth);
// Save the workbook
workbook.Save("LineShapeArrowheadDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
