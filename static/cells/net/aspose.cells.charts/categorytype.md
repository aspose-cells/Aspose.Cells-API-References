##Enum CategoryType
Aspose.Cells.Charts.CategoryType enum. Represents the category axis type
## CategoryType enumeration
Represents the category axis type.
```csharp
public enum CategoryType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| AutomaticScale | `0` | AutomaticScale |
| CategoryScale | `1` | CategoryScale |
| TimeScale | `2` | TimeScale |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class CategoryTypeDemo
{
public static void CategoryTypeExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Adding sample values to cells
worksheet.Cells["A1"].PutValue("Dates");
worksheet.Cells["A2"].PutValue(new DateOnly(2024, 01, 01));
worksheet.Cells["A3"].PutValue(new DateOnly(2024, 03, 01));
worksheet.Cells["A4"].PutValue(new DateOnly(2024, 05, 01));
worksheet.Cells["B1"].PutValue("Data1");
worksheet.Cells["B2"].PutValue(4);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(50);
worksheet.Cells["C1"].PutValue("Data2");
worksheet.Cells["C2"].PutValue(8);
worksheet.Cells["C3"].PutValue(15);
worksheet.Cells["C4"].PutValue(30);
// Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
// Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
// Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("B2:C4", true);
// Setting the category names for the X-axis from the range "A2:A5"
chart.NSeries[0].XValues = "A2:A4";
// Setting the category axis type to TimeScale
chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;
// Setting the major unit scale for the category axis
chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
chart.CategoryAxis.MajorUnit = 2;
// Setting the minor unit scale for the category axis
chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
chart.CategoryAxis.MinorUnit = 2;
// Saving the Excel file
workbook.Save("CategoryTypeExample.xlsx");
workbook.Save("CategoryTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
