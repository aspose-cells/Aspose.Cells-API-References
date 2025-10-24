##ImageOrPrintOptions.SetDesiredSize
ImageOrPrintOptions method. Sets desired width and height of image
## SetDesiredSize(int, int) {#setdesiredsize}
Sets desired width and height of image.
```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```
| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | Int32 | desired width in pixels |
| desiredHeight | Int32 | desired height in pixels |
### Remarks
NOTE: This member is now obsolete. Instead, please use `SetDesiredSize` by setting param keepAspectRatio to false. This property will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample Data");
for (int i = 1; i <= 10; i++)
{
worksheet.Cells["A" + (i + 1)].PutValue(i);
}
// Set print area
worksheet.PageSetup.PrintArea = "A1:A11";
// Create image options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.OnePagePerSheet = true;
options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
// Render worksheet to image
SheetRender render = new SheetRender(worksheet, options);
render.ToImage(0, "output.jpg");
Console.WriteLine("Image generated with desired size 800x600");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## SetDesiredSize(int, int, bool) {#setdesiredsize_1}
Sets desired width and height of image.
```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```
| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | Int32 | desired width in pixels |
| desiredHeight | Int32 | desired height in pixels |
| keepAspectRatio | Boolean | whether to keep aspect ratio of origin image |
### Remarks
The width and height of the output image in pixels will be only based on the set desired width and height.
The [`HorizontalResolution`](../horizontalresolution/) and [`VerticalResolution`](../verticalresolution/) will not effect the width and height of the output image in this case.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32BooleanDemo
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
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
chart.NSeries.CategoryData = "B1:B3";
// Get the chart shape
Shape chartShape = worksheet.Shapes[0];
// Set image options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = ImageType.Png;
options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio
// Save the chart as image
MemoryStream stream = new MemoryStream();
chartShape.ToImage(stream, options);
// Save the image to file
File.WriteAllBytes("output_chart.png", stream.ToArray());
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
