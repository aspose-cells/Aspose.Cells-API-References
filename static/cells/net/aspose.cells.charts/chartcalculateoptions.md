##Class ChartCalculateOptions
Aspose.Cells.Charts.ChartCalculateOptions class. Represents the options for calculating chart
## ChartCalculateOptions class
Represents the options for calculating chart.
```csharp
public class ChartCalculateOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | Creates the options for calculating chart. |
## Properties
| Name | Description |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartCalculateOptionsDemo
{
public static void ChartCalculateOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells[0, 0].PutValue("Category");
worksheet.Cells[0, 1].PutValue("Value");
worksheet.Cells[1, 0].PutValue("A");
worksheet.Cells[1, 1].PutValue(10);
worksheet.Cells[2, 0].PutValue("B");
worksheet.Cells[2, 1].PutValue(20);
worksheet.Cells[3, 0].PutValue("C");
worksheet.Cells[3, 1].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the data range for the chart
chart.SetChartDataRange("A1:B4", true);
// Create an instance of ChartCalculateOptions
ChartCalculateOptions options = new ChartCalculateOptions
{
UpdateAllPoints = true // Set the property to update all data points
};
// Calculate the chart with the specified options
chart.Calculate(options);
// Save the workbook
workbook.Save("ChartCalculateOptionsExample.xlsx");
workbook.Save("ChartCalculateOptionsExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
