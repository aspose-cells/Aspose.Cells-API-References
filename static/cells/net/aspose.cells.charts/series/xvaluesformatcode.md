##Series.XValuesFormatCode
Series property. Represents format code of X Valuess NumberList
## Series.XValuesFormatCode property
Represents format code of X Values's NumberList.
```csharp
public string XValuesFormatCode { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyXValuesFormatCodeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(DateTime.Now);
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
worksheet.Cells["B3"].PutValue(200);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Set XValues format code
chart.NSeries[0].XValuesFormatCode = "M/d/yyyy";
// Save the workbook
workbook.Save("SeriesPropertyXValuesFormatCodeDemo_out.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
