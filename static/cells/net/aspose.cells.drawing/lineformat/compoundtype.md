##LineFormat.CompoundType
LineFormat property. Specifies the line compound type
## LineFormat.CompoundType property
Specifies the line compound type.
```csharp
public MsoLineStyle CompoundType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LineFormatPropertyCompoundTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
// Get the line format
LineFormat lineFmt = line.Line;
// Set compound type
lineFmt.CompoundType = MsoLineStyle.Single;
// Save the workbook
workbook.Save("LineFormatCompoundTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
