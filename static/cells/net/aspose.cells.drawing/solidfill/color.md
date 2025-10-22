##SolidFill.Color
SolidFill property. Gets or sets the Color
## SolidFill.Color property
Gets or sets the Color.
```csharp
public Color Color { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SolidFillPropertyColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a shape to the worksheet with correct parameters
Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
// Set shape properties with color
Color fillColor = Color.LightBlue;
Color textColor = Color.DarkBlue;
string text = "Solid Fill Demo";
// Demonstrate Color property usage
shape.Fill.SolidFill.Color = fillColor;
shape.LineFormat.ForeColor = fillColor;
shape.Text = text;
shape.Font.Color = textColor;
// Save the workbook
workbook.Save("SolidFillPropertyColorDemo.xlsx");
}
}
}
```
### See Also
* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
