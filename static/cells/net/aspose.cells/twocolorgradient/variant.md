##TwoColorGradient.Variant
TwoColorGradient property. Gets and sets the gradient variant
## TwoColorGradient.Variant property
Gets and sets the gradient variant.
```csharp
public int Variant { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
public class TwoColorGradientPropertyVariantDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two-color gradient with initial variant
TwoColorGradient gradient = new TwoColorGradient(
Color.LightBlue,
Color.DarkBlue,
GradientStyleType.Horizontal,
1
);
// Create and apply style to cell A1
Style style1 = workbook.CreateStyle();
style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
worksheet.Cells["A1"].SetStyle(style1);
worksheet.Cells["A1"].PutValue("Variant 1");
// Display current variant value
System.Console.WriteLine("Current Variant value: " + gradient.Variant);
// Modify variant value
gradient.Variant = 2;
// Create and apply modified style to cell B1
Style style2 = workbook.CreateStyle();
style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
worksheet.Cells["B1"].SetStyle(style2);
worksheet.Cells["B1"].PutValue("Variant 2");
// Make cells taller to visualize gradients
worksheet.Cells.Rows[0].Height = 150;
workbook.Save("TwoColorGradientVariantDemo.xlsx");
}
}
}
```
### See Also
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
