##LineFormat.BeginArrowheadWidth
LineFormat property. Gets and sets the begin arrow width type of the line
## LineFormat.BeginArrowheadWidth property
Gets and sets the begin arrow width type of the line.
```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatPropertyBeginArrowheadWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);
// Set the line format properties
LineFormat lineFmt = line.Line;
lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;
// Save the workbook
workbook.Save("LineFormatDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
