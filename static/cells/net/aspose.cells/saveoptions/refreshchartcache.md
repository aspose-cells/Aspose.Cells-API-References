##SaveOptions.RefreshChartCache
SaveOptions property. Indicates whether refreshing chart cache data
## SaveOptions.RefreshChartCache property
Indicates whether refreshing chart cache data
```csharp
public bool RefreshChartCache { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyRefreshChartCacheDemo
{
public static void Run()
{
// Create a sample workbook with a chart
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Create PDF save options with RefreshChartCache enabled
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.RefreshChartCache = true;
// Save the workbook with refresh chart cache option
workbook.Save("output.pdf", pdfSaveOptions);
Console.WriteLine("Workbook saved with chart cache refreshed.");
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
