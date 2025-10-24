##Series.DataLabels
Series property. Represents the DataLabels object for the specified ASeries
## Series.DataLabels property
Represents the DataLabels object for the specified ASeries.
```csharp
public DataLabels DataLabels { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyDataLabelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet and add sample data
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Cells["A1"].PutValue("Products");
dataSheet.Cells["B1"].PutValue("Users");
dataSheet.Cells["A2"].PutValue("Aspose.Cells");
dataSheet.Cells["B2"].PutValue(10000);
dataSheet.Cells["A3"].PutValue("Aspose.Slides");
dataSheet.Cells["B3"].PutValue(8000);
dataSheet.Cells["A4"].PutValue("Aspose.Words");
dataSheet.Cells["B4"].PutValue(12000);
// Add a chart sheet and create a pie chart
Worksheet chartSheet = workbook.Worksheets[workbook.Worksheets.Add(SheetType.Chart)];
Chart chart = chartSheet.Charts[chartSheet.Charts.Add(ChartType.Pie, 7, 0, 20, 6)];
// Add series data and configure data labels
Series series = chart.NSeries[chart.NSeries.Add("=Sheet1!$B$2:$B$4", true)];
series.XValues = "=Sheet1!$A$2:$A$4";
// Configure DataLabels properties
series.DataLabels.ShowValue = true;
series.DataLabels.ShowCategoryName = true;
series.DataLabels.ShowPercentage = true;
series.DataLabels.LinkedSource = null; // Explicitly set to null
// Save the workbook
workbook.Save("SeriesPropertyDataLabelsDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
