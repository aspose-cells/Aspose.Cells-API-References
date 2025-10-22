##Chart.ChangeTemplate
Chart method. Change chart type with preset template
## Chart.ChangeTemplate method
Change chart type with preset template.
```csharp
public void ChangeTemplate(byte[] data)
```
| Parameter | Type | Description |
| --- | --- | --- |
| data | Byte[] | The data of chart template file(.crtx). |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.IO;
public class ChartMethodChangeTemplateWithByteDemo
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
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:B4", false);
// Get template data from another chart file
byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");
try
{
// Call the ChangeTemplate method with byte array parameter
chart.ChangeTemplate(templateData);
Console.WriteLine("Chart template changed successfully using byte array parameter");
// Show effect by saving the workbook
workbook.Save("ChartWithChangedTemplate.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error changing chart template: {ex.Message}");
}
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
