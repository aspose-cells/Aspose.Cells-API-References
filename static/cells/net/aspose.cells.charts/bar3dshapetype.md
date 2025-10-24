##Enum Bar3DShapeType
Aspose.Cells.Charts.Bar3DShapeType enum. Represents the shape used with the 3D bar or column chart
## Bar3DShapeType enumeration
Represents the shape used with the 3-D bar or column chart.
```csharp
public enum Bar3DShapeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Box | `0` | Box |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Cylinder |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class Bar3DShapeTypeDemo
{
public static void Bar3DShapeTypeExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Adding sample values to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Y1");
worksheet.Cells["C4"].PutValue("Y2");
// Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
// Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
// Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
// Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4";
Series series = chart.NSeries[seriesIndex];
// Setting the values of the series
series.Values = "=B1:B4";
// Setting the 3D shape type for the series
series.Bar3DShapeType = Bar3DShapeType.Cylinder;
// Saving the Excel file
workbook.Save("Bar3DShapeTypeExample.xlsx");
workbook.Save("Bar3DShapeTypeExample.pdf");
// Setting the 3D shape type for the series
series.Bar3DShapeType = Bar3DShapeType.ConeToMax;
// Saving the Excel file
workbook.Save("Bar3DShapeTypeExample2.xlsx");
workbook.Save("Bar3DShapeTypeExample2.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
