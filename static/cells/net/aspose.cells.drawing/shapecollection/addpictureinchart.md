##ShapeCollection.AddPictureInChart
ShapeCollection method. Adds a picture to the chart
## ShapeCollection.AddPictureInChart method
Adds a picture to the chart.
```csharp
public Picture AddPictureInChart(int top, int left, Stream stream, int widthScale, int heightScale)
```
| Parameter | Type | Description |
| --- | --- | --- |
| top | Int32 | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | Int32 | Represents the horizontal offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| stream | Stream | Stream object which contains the image data. |
| widthScale | Int32 | Scale of image width, a percentage. |
| heightScale | Int32 | Scale of image height, a percentage. |
### Return Value
Returns a Picture object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts; // Added this using directive
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class ShapeCollectionMethodAddPictureInChartWithInt32Int32StreamInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
chart.NSeries.CategoryData = "B1:B3";
// Create a memory stream with image data
byte[] imageData = File.ReadAllBytes("example.jpg");
MemoryStream stream = new MemoryStream(imageData);
try
{
// Call AddPictureInChart with parameters (Int32, Int32, Stream, Int32, Int32)
Picture picture = chart.Shapes.AddPictureInChart(100, 100, stream, 50, 50);
Console.WriteLine("Picture added to chart successfully. Original dimensions: " +
$"{picture.OriginalWidth}x{picture.OriginalHeight}");
// Save the workbook
workbook.Save("AddPictureInChartDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AddPictureInChart method: {ex.Message}");
}
finally
{
stream.Dispose();
}
}
}
}
```
### See Also
* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
