##TrendlineCollection.Add
TrendlineCollection method. Adds a Trendline object to this collection with specified type
## Add(TrendlineType) {#add}
Adds a [`Trendline`](../../trendline/) object to this collection with specified type.
```csharp
public int Add(TrendlineType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | TrendlineType | Trendline type. |
### Return Value
[`Trendline`](../../trendline/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlineCollectionMethodAddWithTrendlineTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("X");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B1"].PutValue("Y");
worksheet.Cells["B2"].PutValue(2);
worksheet.Cells["B3"].PutValue(4);
worksheet.Cells["B4"].PutValue(8);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series data
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Add exponential trendline to the first series
chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
// Save the workbook
workbook.Save("TrendlineCollectionMethodAddWithTrendlineTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## Add(TrendlineType, string) {#add_1}
Adds a [`Trendline`](../../trendline/) object to this collection with specified type and name.
```csharp
public int Add(TrendlineType type, string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | TrendlineType | Trendline type. |
| name | String | Trendline name. |
### Return Value
[`Trendline`](../../trendline/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlineCollectionMethodAddWithTrendlineTypeStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("X Values");
sheet.Cells["B1"].PutValue("Y Values");
for (int i = 2; i <= 10; i++)
{
sheet.Cells["A" + i].PutValue(i);
sheet.Cells["B" + i].PutValue(i * 2);
}
// Create chart
int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
Chart chart = sheet.Charts[chartIndex];
// Add series and set data
chart.NSeries.Add("B2:B10", true);
chart.NSeries[0].XValues = "A2:A10";
chart.NSeries[0].Name = "Data Series";
// Add trendline with TrendlineType and name
chart.NSeries[0].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic Trend");
// Set some trendline properties
Trendline trendline = chart.NSeries[0].TrendLines[0];
trendline.DisplayEquation = true;
trendline.DisplayRSquared = true;
workbook.Save("TrendlineDemo.xlsx");
}
}
}
```
### See Also
* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
