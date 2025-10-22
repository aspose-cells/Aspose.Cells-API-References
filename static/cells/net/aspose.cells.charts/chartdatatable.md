##Class ChartDataTable
Aspose.Cells.Charts.ChartDataTable class. Represents a chart data table
## ChartDataTable class
Represents a chart data table.
```csharp
public class ChartDataTable
```
## Properties
| Name | Description |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | Gets and sets the display mode of the background |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | Returns a Border object that represents the border of the object |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | Gets a [`Font`](./font/) object which represents the font setting of the specified chart data table. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Obsolete.**) True if the chart data table has horizontal cell borders |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**Obsolete.**) True if the chart data table has outline borders |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**Obsolete.**) True if the chart data table has vertical cell borders |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | True if the chart data table has horizontal cell borders |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | True if the chart data table has outline borders |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | True if the chart data table has vertical cell borders |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | True if the data label legend key is visible. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class ChartDataTableDemo
{
public static void ChartDataTableExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Adding sample values to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
// Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
// Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Displaying the data table
chart.ShowDataTable = true;
// Getting Chart Data Table
ChartDataTable chartTable = chart.ChartDataTable;
// Setting Chart Data Table properties
chartTable.Font.Color = Color.Red;
chartTable.AutoScaleFont = true;
chartTable.BackgroundMode = BackgroundMode.Transparent;
chartTable.HasBorderHorizontal = true;
chartTable.HasBorderVertical = true;
chartTable.HasBorderOutline = true;
chartTable.ShowLegendKey = false;
// Saving the Excel file
workbook.Save("ChartDataTableExample.xlsx");
workbook.Save("ChartDataTableExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
