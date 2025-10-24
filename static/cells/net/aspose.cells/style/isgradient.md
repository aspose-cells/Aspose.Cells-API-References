##Style.IsGradient
Style property. Indicates whether the cell shading is a gradient pattern
## Style.IsGradient property
Indicates whether the cell shading is a gradient pattern.
```csharp
public bool IsGradient { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class StylePropertyIsGradientDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style
Style style = workbook.CreateStyle();
// Set gradient background
style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
// Apply the style to a cell
worksheet.Cells["A1"].SetStyle(style);
// Check if the style has gradient
bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
// Output the result
Console.WriteLine("Cell A1 style has gradient: " + isGradient);
// Save the workbook
workbook.Save("GradientStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
