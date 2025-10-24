##ShapeCollection.AddShapeInChart
ShapeCollection method. Add a shape to chart .All unit is 1/4000 of chart area
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}
Add a shape to chart .All unit is 1/4000 of chart area.
```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top,
int right, int bottom, byte[] imageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The drawing type. |
| placement | PlacementType | the placement type. |
| left | Int32 | In unit of 1/4000 chart area width. |
| top | Int32 | In unit of 1/4000 chart area height. |
| right | Int32 | In unit of 1/4000 chart area width. |
| bottom | Int32 | In unit of 1/4000 chart area height. |
| imageData | Byte[] | If the shape is not a picture or ole object,imageData should be null. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo2
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and create a chart
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(80);
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 15, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
chart.NSeries.CategoryData = "B1:B3";
// Prepare image data
byte[] imageData = File.ReadAllBytes("example.jpg");
try
{
// Call AddShapeInChart with specific parameters
Shape shape = chart.Shapes.AddShapeInChart(
MsoDrawingType.Rectangle,    // Type
PlacementType.Move,          // Placement
100,                         // Left position
100,                         // Top position
1000,                         // Right position
1000,                         // Bottom position
imageData                    // Image data
);
// Set shape properties
shape.Name = "ChartRectangle";
shape.Text = "Shape in Chart";
shape.Fill.SolidFill.Color = System.Drawing.Color.LightBlue;
shape.Line.CompoundType = MsoLineStyle.ThickThin;
shape.Line.Weight = 2; // Medium weight (approximately 2 points)
Console.WriteLine("Shape added to chart successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error adding shape to chart: {ex.Message}");
}
// Save the result
workbook.Save("AddShapeInChartWithMsoDrawingType2.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}
Add a shape to chart .All unit is 1/4000 of chart area.
```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top,
int right, int bottom)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The drawing type. |
| placement | PlacementType | the placement type. |
| left | Int32 | In unit of 1/4000 chart area width. |
| top | Int32 | In unit of 1/4000 chart area height. |
| right | Int32 | In unit of 1/4000 chart area width. |
| bottom | Int32 | In unit of 1/4000 chart area height. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
{
public static void Run()
{
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Add shape to chart
chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
// Set shape text
chart.Shapes[0].Text = "Sample CheckBox";
// Save workbook
workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
