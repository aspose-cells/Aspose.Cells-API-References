##LineShape.BeginArrowheadStyle
LineShape property. Gets and sets the begin arrow head style of the line
## LineShape.BeginArrowheadStyle property
Gets and sets the begin arrow head style of the line.
```csharp
[Obsolete("Use Shape.Line.BeginArrowheadStyle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Line.BeginArrowheadStyle property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineShapePropertyBeginArrowheadStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
LineShape line = worksheet.Shapes.AddLine(5, 0, 5, 5, 50, 150);
// Set different arrowhead styles for demonstration
line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
line.EndArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
// Display the current arrowhead style
Console.WriteLine("Begin Arrowhead Style: " + line.BeginArrowheadStyle);
Console.WriteLine("End Arrowhead Style: " + line.EndArrowheadStyle);
// Save the workbook
workbook.Save("LineShapeArrowheadDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
