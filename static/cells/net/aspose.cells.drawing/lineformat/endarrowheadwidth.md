##LineFormat.EndArrowheadWidth
LineFormat property. Gets and sets the end arrow width type of the line
## LineFormat.EndArrowheadWidth property
Gets and sets the end arrow width type of the line.
```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatPropertyEndArrowheadWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);
// Get the line format
LineFormat lineFmt = line.Line;
// Set the end arrowhead width
lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;
// Save the workbook
workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
