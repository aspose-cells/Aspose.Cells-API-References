##Chart.Style
Chart property. Gets and sets the builtin style
## Chart.Style property
Gets and sets the builtin style.
```csharp
public int Style { get; set; }
```
### Remarks
It should be between 1 and 48. Return -1 if it's not be set.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart1 = worksheet.Charts[chartIndex];
chart1.NSeries.Add("B2:B4", false);
chart1.NSeries.CategoryData = "A2:A4";
// Create another chart and copy the style from first chart
chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 10, 20, 18);
Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex];
chart2.NSeries.Add("B2:B4", false);
chart2.NSeries.CategoryData = "A2:A4";
// Demonstrate Style property usage
chart2.Style = chart1.Style;
// Save the workbook
workbook.Save("ChartStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
