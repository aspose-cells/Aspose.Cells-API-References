##ChartGlobalizationSettings.GetLegendDecreaseName
ChartGlobalizationSettings method. Gets the name of Decrease for Legend
## ChartGlobalizationSettings.GetLegendDecreaseName method
Gets the name of Decrease for Legend.
```csharp
public virtual string GetLegendDecreaseName()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Create globalization settings and get legend decrease name
Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();
// Output the result
Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);
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
