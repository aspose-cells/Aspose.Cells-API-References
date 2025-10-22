##DataLabels.ShowPercentage
DataLabels property. Represents a specified charts data label percentage value display behavior. True displays the percentage value. False to hide
## DataLabels.ShowPercentage property
Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.
```csharp
public bool ShowPercentage { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyShowPercentageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels and show percentage
DataLabels dataLabels = chart.NSeries[0].DataLabels;
dataLabels.ShowPercentage = true;
dataLabels.ShowValue = false;
// Save the workbook
workbook.Save("DataLabelsShowPercentageDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
