##FillFormat.FillType
FillFormat property. Gets and sets fill type
## FillFormat.FillType property
Gets and sets fill type
```csharp
public FillType FillType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyFillTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
// Set solid fill with color
shape.Fill.FillType = FillType.Solid;
shape.Fill.SolidFill.Color = System.Drawing.Color.Red;
// Output the fill type
Console.WriteLine("Shape fill type: " + shape.Fill.FillType);
// Change to gradient fill
shape.Fill.FillType = FillType.Gradient;
Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);
// Save the workbook
workbook.Save("FillTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
