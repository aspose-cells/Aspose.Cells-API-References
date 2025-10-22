##MsoFillFormat.ForeColor
MsoFillFormat property. Gets and sets the fill fore color
## MsoFillFormat.ForeColor property
Gets and sets the fill fore color.
```csharp
public Color ForeColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MsoFillFormatPropertyForeColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);
// Get the fill format
MsoFillFormat fillFormat = rectangle.FillFormat;
// Set and demonstrate ForeColor property
fillFormat.ForeColor = System.Drawing.Color.Red;
Console.WriteLine("ForeColor set to: " + fillFormat.ForeColor);
// Modify the ForeColor
fillFormat.ForeColor = System.Drawing.Color.FromArgb(0, 128, 255);
Console.WriteLine("ForeColor changed to: " + fillFormat.ForeColor);
// Save the workbook
workbook.Save("MsoFillFormatForeColorDemo.xlsx");
}
}
}
```
### See Also
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
