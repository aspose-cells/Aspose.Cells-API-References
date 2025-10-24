##Enum GradientFillType
Aspose.Cells.Drawing.GradientFillType enum. Represents all Gradient fill type
## GradientFillType enumeration
Represents all Gradient fill type.
```csharp
public enum GradientFillType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Linear | `0` | Linear |
| Radial | `1` | Radial |
| Rectangle | `2` | Rectangle |
| Path | `3` | Path |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassGradientFillTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to demonstrate gradient fill
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);
// Get the fill format
FillFormat fillFormat = shape.Fill;
// Set gradient fill type and properties
fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);
// Output gradient direction type
Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);
// Save the workbook
workbook.Save("GradientFillTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
