##Series.Bar3DShapeType
Series property. Gets or sets the 3D shape type used with the 3D bar or column chart
## Series.Bar3DShapeType property
Gets or sets the 3D shape type used with the 3-D bar or column chart.
```csharp
public Bar3DShapeType Bar3DShapeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyBar3DShapeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a 3D bar chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set the bar shape type to Cylinder
chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.Cylinder;
// Save the workbook
workbook.Save("Bar3DShapeTypeDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [Bar3DShapeType](../../bar3dshapetype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
