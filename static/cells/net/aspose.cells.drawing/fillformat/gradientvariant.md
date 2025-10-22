##FillFormat.GradientVariant
FillFormat property. Returns the gradient variant for the specified fill. Only applies for Excel 2007
## FillFormat.GradientVariant property
Returns the gradient variant for the specified fill. Only applies for Excel 2007.
```csharp
public int GradientVariant { get; }
```
### Remarks
Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyGradientVariantDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 150);
FillFormat fillFormat = rectangle.Fill;
fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 2);
Console.WriteLine("GradientVariant after SetTwoColorGradient: " + fillFormat.GradientVariant);
fillFormat.SetPresetColorGradient(GradientPresetType.Gold, GradientStyleType.FromCorner, 4);
Console.WriteLine("GradientVariant after SetPresetColorGradient: " + fillFormat.GradientVariant);
}
}
}
```
### See Also
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
