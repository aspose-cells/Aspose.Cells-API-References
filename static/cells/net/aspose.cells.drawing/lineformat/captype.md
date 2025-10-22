##LineFormat.CapType
LineFormat property. Specifies the ending caps
## LineFormat.CapType property
Specifies the ending caps.
```csharp
public LineCapType CapType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatPropertyCapTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);
// Set line format properties
LineFormat lineFmt = line.Line;
lineFmt.CapType = LineCapType.Flat;
// Save the workbook
workbook.Save("LineFormatCapTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
