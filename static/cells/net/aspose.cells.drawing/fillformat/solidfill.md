##FillFormat.SolidFill
FillFormat property. Gets SolidFill object
## FillFormat.SolidFill property
Gets `SolidFill` object.
```csharp
public SolidFill SolidFill { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertySolidFillDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
// Set solid fill color for the shape
shape.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(135, 222, 255);
// Get and display the solid fill color
System.Drawing.Color fillColor = shape.Fill.SolidFill.Color;
Console.WriteLine("Solid Fill Color - R:{0}, G:{1}, B:{2}",
fillColor.R, fillColor.G, fillColor.B);
// Save the workbook
workbook.Save("SolidFillDemo.xlsx");
}
}
}
```
### See Also
* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
