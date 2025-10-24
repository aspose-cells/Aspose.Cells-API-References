##Axis.LogBase
Axis property. Represents the logarithmic base. Default value is 10.Only applies for Excel2007
## Axis.LogBase property
Represents the logarithmic base. Default value is 10.Only applies for Excel2007.
```csharp
public double LogBase { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyLogBaseDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("X Values");
worksheet.Cells["B1"].PutValue("Y Values");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells[$"A{i}"].PutValue(Math.Pow(2, i-2)); // Exponential values
worksheet.Cells[$"B{i}"].PutValue(i * 10);
}
// Create a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add($"B2:B10", true);
chart.NSeries[0].XValues = $"A2:A10";
chart.NSeries[0].Name = "Logarithmic Series";
// Configure logarithmic axis
chart.CategoryAxis.IsLogarithmic = true;
chart.CategoryAxis.LogBase = 2; // Set logarithmic base to 2
chart.CategoryAxis.Title.Text = "Logarithmic Scale (Base 2)";
// Save the workbook
workbook.Save("AxisPropertyLogBaseDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
