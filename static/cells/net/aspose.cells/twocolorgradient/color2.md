##TwoColorGradient.Color2
TwoColorGradient property. Gets and sets the second gradient color
## TwoColorGradient.Color2 property
Gets and sets the second gradient color.
```csharp
public Color Color2 { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
public class TwoColorGradientPropertyColor2Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a two-color gradient instance
TwoColorGradient gradient = new TwoColorGradient(
Color.LightBlue,
Color.Green,
GradientStyleType.Horizontal,
1);
// Create first style with initial gradient
Style style1 = workbook.CreateStyle();
style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
worksheet.Cells["A1"].PutValue("Initial Gradient");
worksheet.Cells["A1"].SetStyle(style1);
// Display current Color2 value
System.Console.WriteLine("Current Color2: " + gradient.Color2);
// Modify Color2 property
gradient.Color2 = Color.Red;
// Create second style with modified gradient
Style style2 = workbook.CreateStyle();
style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
worksheet.Cells["A2"].PutValue("Modified Gradient");
worksheet.Cells["A2"].SetStyle(style2);
// Adjust rows for visibility
worksheet.Cells.SetRowHeight(0, 40);
worksheet.Cells.SetRowHeight(1, 40);
// Save the workbook
workbook.Save("TwoColorGradientColor2Demo.xlsx");
}
}
}
```
### See Also
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
