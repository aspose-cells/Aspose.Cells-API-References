##Enum QuartileCalculationType
Aspose.Cells.Charts.QuartileCalculationType enum. Represents quartile calculation methods
## QuartileCalculationType enumeration
Represents quartile calculation methods.
```csharp
public enum QuartileCalculationType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Exclusive | `0` | The quartile calculation includes the median when splitting the dataset into quartiles. |
| Inclusive | `1` | The quartile calculation excludes the median when splitting the dataset into quartiles. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class QuartileCalculationTypeDemo
{
public static void QuartileCalculationTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["A5"].PutValue("Q4");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Access the series layout properties
SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;
// Set the quartile calculation type
layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;
// Save the workbook
workbook.Save("QuartileCalculationTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
