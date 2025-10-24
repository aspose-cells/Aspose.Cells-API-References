##ChartGlobalizationSettings.GetChartTitleName
ChartGlobalizationSettings method. Gets the name of Chart Title
## ChartGlobalizationSettings.GetChartTitleName method
Gets the name of Chart Title.
```csharp
public virtual string GetChartTitleName()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartGlobalizationSettingsMethodGetChartTitleNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["A3"].PutValue("Category 3");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Create an instance of ChartGlobalizationSettings
ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
// Demonstrate the usage of GetChartTitleName method
string chartTitleName = globalizationSettings.GetChartTitleName();
Console.WriteLine("Chart Title Name: " + chartTitleName);
// Save the workbook
workbook.Save("ChartGlobalizationSettingsExample.xlsx");
}
}
}
```
### See Also
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
