##DataLabels.ShowLegendKey
DataLabels property. Represents a specified charts data label legend key display behavior. True if the data label legend key is visible
## DataLabels.ShowLegendKey property
Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.
```csharp
public bool ShowLegendKey { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyShowLegendKeyDemo
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
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get data labels
DataLabels dataLabels = chart.NSeries[0].DataLabels;
// Set ShowLegendKey to true
dataLabels.ShowLegendKey = true;
Console.WriteLine("ShowLegendKey set to: " + dataLabels.ShowLegendKey);
// Save the workbook
workbook.Save("DataLabelsShowLegendKeyDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
