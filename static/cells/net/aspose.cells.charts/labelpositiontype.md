##Enum LabelPositionType
Aspose.Cells.Charts.LabelPositionType enum. Represents data label position type
## LabelPositionType enumeration
Represents data label position type.
```csharp
public enum LabelPositionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Center | `0` | Applies only to bar, 2d/3d pie charts |
| InsideBase | `1` | Applies only to bar, 2d/3d pie charts |
| InsideEnd | `2` | Applies only to bar charts |
| OutsideEnd | `3` | Applies only to bar, 2d/3d pie charts |
| Above | `4` | Applies only to line charts |
| Below | `5` | Applies only to line charts |
| Left | `6` | Applies only to line charts |
| Right | `7` | Applies only to line charts |
| BestFit | `8` | Applies only to 2d/3d pie charts |
| Moved | `9` | User moved the data labels, Only for reading chart from template file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class LabelPositionTypeDemo
{
public static void LabelPositionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add the data series to the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the data labels of the first series
DataLabels dataLabels = chart.NSeries[0].DataLabels;
// Set the position of the data labels
dataLabels.Position = LabelPositionType.InsideBase;
// Show the category name in the data labels
dataLabels.ShowCategoryName = true;
// Show the value in the data labels
dataLabels.ShowValue = true;
// Save the workbook
workbook.Save("LabelPositionTypeExample.xlsx");
workbook.Save("LabelPositionTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
