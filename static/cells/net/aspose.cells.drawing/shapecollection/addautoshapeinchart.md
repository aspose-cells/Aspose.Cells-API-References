##ShapeCollection.AddAutoShapeInChart
ShapeCollection method. Adds a AutoShape to the chart
## ShapeCollection.AddAutoShapeInChart method
Adds a AutoShape to the chart.
```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | AutoShapeType | Auto shape type. |
| top | Int32 | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | Int32 | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | Int32 | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | Int32 | Represents the width of textbox, in units of 1/4000 of the chart area. |
### Return Value
Returns a shape object.
### Remarks
The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
try
{
// Call the AddAutoShapeInChart method to add a star shape to the chart
Shape shape = chart.Shapes.AddAutoShapeInChart(
AutoShapeType.Star16,  // AutoShapeType
100,                  // Top position (in pixels)
100,                  // Left position (in pixels)
200,                  // Height (in pixels)
200);                 // Width (in pixels)
// Set shape properties
shape.Name = "SampleStar";
shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
shape.Line.SolidFill.Color = System.Drawing.Color.Red;
Console.WriteLine("Star shape added successfully to the chart.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
}
// Save the result
workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
