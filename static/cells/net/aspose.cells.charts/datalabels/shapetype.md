##DataLabels.ShapeType
DataLabels property. Gets or sets shape type of data label
## DataLabels.ShapeType property
Gets or sets shape type of data label.
```csharp
public DataLabelShapeType ShapeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyShapeTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
Series series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
DataLabels dataLabels = series.DataLabels;
dataLabels.ShapeType = DataLabelShapeType.Rect;
Console.WriteLine("ShapeType set to: " + dataLabels.ShapeType);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [DataLabelShapeType](../../../aspose.cells.drawing/datalabelshapetype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
