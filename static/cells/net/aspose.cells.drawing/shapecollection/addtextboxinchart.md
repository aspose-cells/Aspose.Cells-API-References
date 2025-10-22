##ShapeCollection.AddTextBoxInChart
ShapeCollection method. Adds a textbox to the chart
## ShapeCollection.AddTextBoxInChart method
Adds a textbox to the chart.
```csharp
public TextBox AddTextBoxInChart(int top, int left, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| top | Int32 | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | Int32 | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | Int32 | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | Int32 | Represents the width of textbox, in units of 1/4000 of the chart area. |
### Return Value
A TextBox object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddTextBoxInChartWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart waterfallChart = worksheet.Charts[chartIndex];
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Categories");
cells["A2"].PutValue("Start");
cells["A3"].PutValue("Positive Value 1");
cells["A4"].PutValue("Negative Value 1");
cells["A5"].PutValue("Positive Value 2");
cells["A6"].PutValue("End");
waterfallChart.NSeries.CategoryData = "A2:A6";
cells["B1"].PutValue("Values");
cells["B2"].PutValue(0);
cells["B3"].PutValue(20);
cells["B4"].PutValue(-10);
cells["B5"].PutValue(15);
cells["B6"].PutValue(25);
waterfallChart.NSeries.Add("B2:B6", true);
Shape textBox = waterfallChart.Shapes.AddTextBoxInChart(100, 100, 200, 50);
textBox.Text = "Sample TextBox in Chart";
textBox.Font.Color = Color.Blue;
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
