##Chart.ToImage
Chart method. Gets a 32bit Bitmap object of the chart
## ToImage() {#toimage}
Gets a 32-bit `Bitmap` object of the chart.
```csharp
public Bitmap ToImage()
```
### Return Value
the picture of the chart.
### Remarks
If the width or height is zero or the chart is not supported according to Supported Charts List, it will return null.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ChartMethodToImageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Fruits");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1200);
worksheet.Cells["B3"].PutValue(800);
worksheet.Cells["B4"].PutValue(1500);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:B4", true);
// Convert chart to image and save to file
chart.ToImage("ChartImage.png", ImageType.Png);
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(ImageOrPrintOptions) {#toimage_1}
Gets a 32-bit `Bitmap` object of the chart. `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression and ImageOrPrintOptions.Quality attributes are ignored.
```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | Additional image creation options |
### Return Value
the picture of the chart.
### Remarks
Returns a 32-bit bitmap object, so ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression and ImageOrPrintOptions.Quality attributes do not affect the method. If the width or height is zero or the chart is not supported according to Supported Charts List, it will return null.
### Examples
Gets a bitmap object with 200 x dpi and 300 y dpi.
```csharp
[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 200;
options.VerticalResolution = 300;
Workbook book = new Workbook(@"test.xls");
Bitmap chartObject = book.Worksheets[0].Charts[0].ToImage(options);
[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions()
options.HorizontalResolution = 200
options.VerticalResolution = 300
Dim book As Workbook =  New Workbook("test.xls")
Dim chartObject As Bitmap = book.Worksheets(0).Charts(0).ToImage(options)
```
### See Also
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(string) {#toimage_6}
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```csharp
public void ToImage(string imageFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
### Remarks
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodToImageWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["A3"].PutValue("Vegetables");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(45);
worksheet.Cells["B3"].PutValue(55);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Save chart as image
chart.ToImage("ChartImage.jpg");
Console.WriteLine("Chart saved as image successfully.");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(string, ImageFormat) {#toimage_10}
Creates the chart image and saves it to a file in the specified format.
```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| imageFormat | ImageFormat | The format in which to save the image. |
### Remarks
NOTE: This member is now obsolete. Instead, please use Chart.ToImage(string, ImageType) method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(string, ImageType) {#toimage_7}
Creates the chart image and saves it to a file in the specified image type.
```csharp
public void ToImage(string imageFile, ImageType imageType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| imageType | ImageType | The image type in which to save the image. |
### Remarks
The type of the image is specified by using `imageType`. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodToImageWithStringImageTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(15);
worksheet.Cells["B4"].PutValue(7);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Save chart to image with specified ImageType
chart.ToImage("output_chart.png", ImageType.Png);
Console.WriteLine("Chart saved to image successfully.");
}
}
}
```
### See Also
* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(string, long) {#toimage_9}
Creates the chart image and saves it to a file in the Jpeg format.
```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| jpegQuality | Int64 | Jpeg quality. |
### Remarks
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. NOTE: This method is now obsolete. Instead, please use ToImage(string,ImageOrPrintOptions) method with specified quality. This method will be removed 12 months later since March 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartMethodToImageWithStringInt64Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["A3"].PutValue("Vegetables");
worksheet.Cells["A4"].PutValue("Grains");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["B4"].PutValue(20);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
try
{
// Call the ToImage method with parameters (String, Int64)
string imagePath = "ChartImage.jpg";
long jpegQuality = 90; // Quality percentage (0-100)
chart.ToImage(imagePath, jpegQuality);
Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ToImage method: {ex.Message}");
}
// Save the workbook
workbook.Save("ChartToImageDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(Stream, long) {#toimage_4}
Creates the chart image and saves it to a stream in the Jpeg format.
```csharp
public void ToImage(Stream stream, long jpegQuality)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| jpegQuality | Int64 | Jpeg quality. |
### Remarks
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(Stream, ImageFormat) {#toimage_5}
Creates the chart image and saves it to a stream in the specified format.
```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| imageFormat | ImageFormat | The format in which to save the image. |
### Remarks
NOTE: This member is now obsolete. Instead, please use Chart.ToImage(Stream, ImageType) method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(Stream, ImageType) {#toimage_2}
Creates the chart image and saves it to a stream in the specified format.
```csharp
public void ToImage(Stream stream, ImageType imageType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| imageType | ImageType | The image type in which to save the image. |
### Remarks
The type of the image is specified by using `imageType`. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
### See Also
* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(string, ImageOrPrintOptions) {#toimage_8}
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| options | ImageOrPrintOptions | Additional image creation options |
### Remarks
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodToImageWithStringImageOrPrintOptionsDemo
{
public static void Run()
{
// Create image options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.TiffCompression = TiffCompression.CompressionCCITT4;
// Load the workbook
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
// Save chart to image
chart.ToImage("chart.tiff", options);
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}
Creates the chart image and saves it to a stream in the specified format.
```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| options | ImageOrPrintOptions | Additional image creation options |
### Remarks
The type of the image is specified by using `options.ImageType`. The following formats are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.
### See Also
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
