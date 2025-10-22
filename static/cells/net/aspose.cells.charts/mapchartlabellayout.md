##Enum MapChartLabelLayout
Aspose.Cells.Charts.MapChartLabelLayout enum. Represents the layout of map charts labels
## MapChartLabelLayout enumeration
Represents the layout of map chart's labels.
```csharp
public enum MapChartLabelLayout
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| BestFitOnly | `0` | Only best fit. |
| ShowAll | `1` | Shows all labels. |
| None | `2` | No labels. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class MapChartLabelLayoutDemo
{
public static void MapChartLabelLayoutExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the map chart
worksheet.Cells["A1"].PutValue("Country");
worksheet.Cells["A2"].PutValue("USA");
worksheet.Cells["A3"].PutValue("Canada");
worksheet.Cells["A4"].PutValue("Mexico");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(150);
// Add a map chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set the data range for the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the series layout properties
SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;
// Set the map chart label layout
layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
// Save the workbook
workbook.Save("MapChartLabelLayoutExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
