##LineShape.EndArrowheadStyle
LineShape property. Gets and sets the end arrow head style of the line
## LineShape.EndArrowheadStyle property
Gets and sets the end arrow head style of the line.
```csharp
[Obsolete("Use Shape.Line.EndArrowheadStyle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line.EndArrowheadStyle property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineShapePropertyEndArrowheadStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
LineShape line = worksheet.Shapes.AddLine(5, 0, 5, 5, 50, 150);
// Set different end arrowhead styles
line.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
Console.WriteLine("Line EndArrowheadStyle set to: ArrowOpen");
// Change the end arrowhead style
line.EndArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
Console.WriteLine("Line EndArrowheadStyle changed to: ArrowStealth");
// Save the workbook
workbook.Save("LineShapeEndArrowheadStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
