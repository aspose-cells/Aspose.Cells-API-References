##LineShape.EndArrowheadWidth
LineShape property. Gets and sets the end arrow head width of the line
## LineShape.EndArrowheadWidth property
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
public class LineShapePropertyEndArrowheadWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
LineShape line = worksheet.Shapes.AddLine(5, 0, 5, 5, 100, 150);
// Set line properties including EndArrowheadWidth
line.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
line.EndArrowheadWidth = MsoArrowheadWidth.Wide;
// Display the EndArrowheadWidth value
Console.WriteLine("EndArrowheadWidth: " + line.EndArrowheadWidth);
// Save the workbook
workbook.Save("LineShapePropertyEndArrowheadWidthDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
