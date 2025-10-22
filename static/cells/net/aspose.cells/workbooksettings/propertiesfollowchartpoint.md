##WorkbookSettings.PropertiesFollowChartPoint
WorkbookSettings property. Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference
## WorkbookSettings.PropertiesFollowChartPoint property
Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference.
```csharp
public bool PropertiesFollowChartPoint { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyPropertiesFollowChartPointDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
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
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set PropertiesFollowChartPoint to true
workbook.Settings.PropertiesFollowChartPoint = true;
// Save the workbook
workbook.Save("output.xlsx");
// Verify the setting was saved
Workbook loadedWorkbook = new Workbook("output.xlsx");
Console.WriteLine("PropertiesFollowChartPoint: " + loadedWorkbook.Settings.PropertiesFollowChartPoint);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
