##FillFormat.GradientColor1
FillFormat property. Returns the gradient color 1 for the specified fill
## FillFormat.GradientColor1 property
Returns the gradient color 1 for the specified fill.
```csharp
public Color GradientColor1 { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyGradientColor1Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Get fill format of first series
FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
// Create gradient fill using correct parameter types
fillFormat.SetTwoColorGradient(
Color.Red,
Color.White,
GradientStyleType.Horizontal,
1); // Gradient variant must be integer (1-4)
// Get and display gradient color
Color gradientColor1 = fillFormat.GradientColor1;
Console.WriteLine("Gradient Color 1: " + gradientColor1);
Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
