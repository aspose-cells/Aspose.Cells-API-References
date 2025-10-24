##DataLabels.Font
DataLabels property. Gets the font of the DataLabels
## DataLabels.Font property
Gets the font of the DataLabels;
```csharp
public override Font Font { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels
Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
dataLabels.ShowValue = true;
// Set font properties
dataLabels.Font.Color = Color.Red;
dataLabels.Font.Size = 14;
dataLabels.Font.IsBold = true;
dataLabels.Font.Name = "Arial";
// Save the workbook
workbook.Save("DataLabelsFontDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
