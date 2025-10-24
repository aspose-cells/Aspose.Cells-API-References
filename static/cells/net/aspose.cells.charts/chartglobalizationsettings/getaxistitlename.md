##ChartGlobalizationSettings.GetAxisTitleName
ChartGlobalizationSettings method. Gets the name of Title for Axis
## ChartGlobalizationSettings.GetAxisTitleName method
Gets the name of Title for Axis.
```csharp
public virtual string GetAxisTitleName()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartGlobalizationSettingsMethodGetAxisTitleNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Create globalization settings and get axis title name
ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
string axisTitleName = globalizationSettings.GetAxisTitleName();
// Set the axis title
chart.ValueAxis.Title.Text = axisTitleName;
chart.CategoryAxis.Title.Text = axisTitleName;
// Output the axis title name
Console.WriteLine("Axis Title Name: " + axisTitleName);
// Save the workbook
workbook.Save("ChartGlobalizationSettingsDemo.xlsx");
}
}
}
```
### See Also
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
