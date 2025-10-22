##DataLabels.ApplyFont
DataLabels method. Apply the font of the datalabels to all child nodes
## DataLabels.ApplyFont method
Apply the font of the datalabels to all child nodes.
```csharp
public void ApplyFont()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataLabelsMethodApplyFontDemo
{
public static void Run()
{
// Create a workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["A5"].PutValue("D");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Show data labels
Series series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
// Set new font color for data labels
Color newColor = Color.Green;
series.DataLabels.Font.Color = newColor;
// Apply the font settings to all data labels
series.DataLabels.ApplyFont();
// Save the workbook
workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
