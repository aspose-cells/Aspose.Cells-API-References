##FillFormat.GradientColor2
FillFormat property. Returns the gradient color 2 for the specified fill
## FillFormat.GradientColor2 property
Returns the gradient color 2 for the specified fill.
```csharp
public Color GradientColor2 { get; }
```
### Remarks
Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyGradientColor2Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create rectangle shape with two-color gradient fill
Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
FillFormat fill = rectangle.Fill;
fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);
// Verify gradient color properties
Console.WriteLine("GradientColor2: " + fill.GradientColor2);
}
}
}
```
### See Also
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
