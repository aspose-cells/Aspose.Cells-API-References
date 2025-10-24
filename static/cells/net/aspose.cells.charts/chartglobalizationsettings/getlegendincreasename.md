##ChartGlobalizationSettings.GetLegendIncreaseName
ChartGlobalizationSettings method. Gets the name of increase for Legend
## ChartGlobalizationSettings.GetLegendIncreaseName method
Gets the name of increase for Legend.
```csharp
public virtual string GetLegendIncreaseName()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Create globalization settings and get legend increase name
ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
// Output the result
Console.WriteLine("Legend Increase Name: " + legendIncreaseName);
// Save the workbook
workbook.Save("ChartGlobalizationDemo.xlsx");
}
}
}
```
### See Also
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
