##LineFormat.EndArrowheadLength
LineFormat property. Gets and sets the end arrow length type of the line
## LineFormat.EndArrowheadLength property
Gets and sets the end arrow length type of the line.
```csharp
public MsoArrowheadLength EndArrowheadLength { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatPropertyEndArrowheadLengthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape and get the shape object directly
LineShape line = (LineShape)worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);
// Set end arrowhead length
line.Line.EndArrowheadLength = MsoArrowheadLength.Long;
// Save the workbook
workbook.Save("LineFormatPropertyEndArrowheadLengthDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
