##DataLabels.Border
DataLabels property. Gets the border
## DataLabels.Border property
Gets the [`border`](../../../aspose.cells.drawing/line/).
```csharp
public override Line Border { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyBorderDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Fruit");
sheet.Cells["A2"].PutValue(50);
sheet.Cells["B1"].PutValue("Vegetables");
sheet.Cells["B2"].PutValue(30);
sheet.Cells["C1"].PutValue("Dairy");
sheet.Cells["C2"].PutValue(20);
int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 5, 20, 20);
Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("A2:C2", false);
chart.NSeries.CategoryData = "A1:C1";
DataLabels labels = chart.NSeries[0].DataLabels;
labels.ShowCategoryName = true;
labels.ShowPercentage = true;
labels.Border.Color = Color.Red;
workbook.Save("DataLabelsBorderDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
