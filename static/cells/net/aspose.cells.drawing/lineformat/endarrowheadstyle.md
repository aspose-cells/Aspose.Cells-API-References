##LineFormat.EndArrowheadStyle
LineFormat property. Gets and sets the end arrow type of the line
## LineFormat.EndArrowheadStyle property
Gets and sets the end arrow type of the line.
```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatPropertyEndArrowheadStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);
// Get the line format
LineFormat lineFmt = line.Line;
// Set the end arrowhead style
lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
// Save the workbook
workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
