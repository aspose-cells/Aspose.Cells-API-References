##ShapeCollection.AddLabelInChart
ShapeCollection method. Adds a label to the chart
## ShapeCollection.AddLabelInChart method
Adds a label to the chart.
```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| top | Int32 | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| left | Int32 | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| height | Int32 | Represents the height of label, in units of 1/4000 of the chart area. |
| width | Int32 | Represents the width of label, in units of 1/4000 of the chart area. |
### Return Value
A new Label object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
try
{
// Call AddLabelInChart method with parameters (top, left, height, width)
Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
// Set label properties
label.Text = "Sample Chart Label";
label.Font.Color = System.Drawing.Color.Red;
label.Font.Size = 12;
Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
}
// Save the result
workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
