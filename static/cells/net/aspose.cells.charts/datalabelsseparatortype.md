##Enum DataLabelsSeparatorType
Aspose.Cells.Charts.DataLabelsSeparatorType enum. Represents the separator type of DataLabels
## DataLabelsSeparatorType enumeration
Represents the separator type of DataLabels.
```csharp
public enum DataLabelsSeparatorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Auto | `0` | Represents automatic separator |
| Space | `1` | Represents space(" ") |
| Comma | `2` | Represents comma(",") |
| Semicolon | `3` | Represents semicolon(";") |
| Period | `4` | Represents period(".") |
| NewLine | `5` | Represents newline("\n") |
| Custom | `6` | Represents custom separator |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class DataLabelsSeparatorTypeDemo
{
public static void DataLabelsSeparatorTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data for the chart
worksheet.Cells[0, 0].PutValue("Category");
worksheet.Cells[0, 1].PutValue("Value");
worksheet.Cells[1, 0].PutValue("A");
worksheet.Cells[1, 1].PutValue(10);
worksheet.Cells[2, 0].PutValue("B");
worksheet.Cells[2, 1].PutValue(20);
worksheet.Cells[3, 0].PutValue("C");
worksheet.Cells[3, 1].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add the data series to the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the data labels of the first series
DataLabels dataLabels = chart.NSeries[0].DataLabels;
// Set the separator type to comma
dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
// Enable data labels and set some properties
dataLabels.ShowCategoryName = true;
dataLabels.ShowValue = true;
dataLabels.Position = LabelPositionType.InsideBase;
// Set font properties
dataLabels.Font.Color = Color.Blue;
dataLabels.Font.IsBold = true;
// Save the workbook
workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
workbook.Save("DataLabelsSeparatorTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
