##DataLabels.ShowCategoryName
DataLabels property. Represents a specified charts data label category name display behavior.True to display the category name for the data labels on a chart. False to hide
## DataLabels.ShowCategoryName property
Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide.
```csharp
public bool ShowCategoryName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyShowCategoryNameDemo
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
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels and set properties
DataLabels dataLabels = chart.NSeries[0].DataLabels;
dataLabels.ShowValue = true;
dataLabels.ShowCategoryName = true;
dataLabels.SeparatorType = DataLabelsSeparatorType.Semicolon;
// Save the workbook
workbook.Save("DataLabelsShowCategoryNameDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
