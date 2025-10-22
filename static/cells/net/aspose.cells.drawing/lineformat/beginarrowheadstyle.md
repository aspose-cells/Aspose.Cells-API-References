##LineFormat.BeginArrowheadStyle
LineFormat property. Gets and sets the begin arrow type of the line
## LineFormat.BeginArrowheadStyle property
Gets and sets the begin arrow type of the line.
```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatPropertyBeginArrowheadStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);
// Set the begin arrowhead style
line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;
// Save the workbook
workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
