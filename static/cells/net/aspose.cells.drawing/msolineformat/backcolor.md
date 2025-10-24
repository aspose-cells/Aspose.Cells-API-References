##MsoLineFormat.BackColor
MsoLineFormat property. Gets and sets the border line back color
## MsoLineFormat.BackColor property
Gets and sets the border line back color.
```csharp
public Color BackColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MsoLineFormatPropertyBackColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
// Set line properties
line.LineFormat.ForeColor = Color.Red;
line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
line.LineFormat.Weight = 2.0;
// Save the workbook
workbook.Save("LineFormatBackColorDemo.xlsx");
}
}
}
```
### See Also
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
