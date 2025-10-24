##LineFormat.BeginArrowheadLength
LineFormat property. Gets and sets the begin arrow length type of the line
## LineFormat.BeginArrowheadLength property
Gets and sets the begin arrow length type of the line.
```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatPropertyBeginArrowheadLengthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
LineShape line = (LineShape)lineShape;
// Set the begin arrowhead length
line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;
// Save the workbook
workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
