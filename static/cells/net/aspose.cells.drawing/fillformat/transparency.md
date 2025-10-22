##FillFormat.Transparency
FillFormat property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
## FillFormat.Transparency property
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate transparency
Shape shape = worksheet.Shapes.AddRectangle(10, 10, 200, 100, 50, 50);
// Set fill properties with transparency
shape.Fill.FillType = FillType.Solid;
shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
shape.Fill.Transparency = 0.3; // 30% transparent
// Save the workbook
workbook.Save("FillFormatTransparencyDemo.xlsx");
}
}
}
```
### See Also
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
