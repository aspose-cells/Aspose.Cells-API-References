---
title: Chart.ToImage
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Gets a 32bit Bitmap object of the chart
type: docs
url: /net/aspose.cells.charts/chart/toimage/
---
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
// Called: Bitmap bitmap = charts[0].ToImage();
public void Chart_Method_ToImage()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "HideCatergoryData.xls");
    ChartCollection charts = workbook.Worksheets[0].Charts;
    Bitmap bitmap = charts[0].ToImage();
    bitmap.Save(Constants.destPath + "HideCatergoryData.bmp", ImageFormat.Bmp);
}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

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

---

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
// Called: ch.ToImage(destpath + "CELLSNET-30877_" + i + ".jpg");
        //http://www.aspose.com/community/forums/thread/324870/dates-in-chart-converted-to-image-show-as-serial-number-not-date.aspx
        public void Chart_Method_ToImage()
        {

            Console.WriteLine("testCELLSNET_30877()");
            string infn = path + @"example.xlsm";
            string outfn = destpath + @"EVALJBVersion2.out.xlsm";

            Workbook wb = new Workbook(infn);

            wb.Save(outfn);

            wb = new Workbook(outfn);

            Worksheet ws = wb.Worksheets["RMA Charts"];

            int i = 0;

            foreach (Chart ch in ws.Charts)
            {
                i++;
                ch.ToImage(destpath + "CELLSNET-30877_" + i + ".jpg");
            }
#if WTEST
            Process.Start("explorer.exe", string.Format("\"{0}\"", outfn));
#endif
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

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

### Examples

```csharp
namespace AsposeCellsExamples.ChartMethodToImageWithStringImageFormatDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartMethodToImageWithStringImageFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Set chart data range
            chart.SetChartDataRange("A1:B3", true);
            
            try
            {
                // Call the ToImage method with parameters (String, ImageType)
                chart.ToImage("output.png", ImageType.Png);
                
                Console.WriteLine("Chart successfully exported to image file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error exporting chart to image: {ex.Message}");
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

---

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
// Called: chart.ToImage(Constants.PIVOT_CHECK_FILE_PATH
        public void Chart_Method_ToImage()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET43750_";

            Aspose.Cells.LoadOptions loadOptions = new Aspose.Cells.LoadOptions(LoadFormat.Xlsx);
            Workbook workbook = new Workbook(filePath + "Template.xlsx");
            Worksheet worksheet = workbook.Worksheets[1];
            workbook.CalculateFormula();
            foreach (PivotTable pivotTable in workbook.Worksheets[2].PivotTables)
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + "example.xlsx");
            int index = 0;
            foreach (Chart chart in workbook.Worksheets[0].Charts)
            {
                chart.RefreshPivotData();
#if !NETCOREAPP2_0
                chart.ToImage(Constants.PIVOT_CHECK_FILE_PATH
                    + "NET43750_out_" + index.ToString() + ".png", ImageType.Png);
#else 
                chart.ToImage(Constants.PIVOT_CHECK_FILE_PATH + "NET43750_out_" + index.ToString() + ".bmp");
#endif
                index += 1;
            }

           
        }
```

### See Also

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

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
namespace AsposeCellsExamples.ChartMethodToImageWithStringInt64Demo
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

---

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

### Examples

```csharp
namespace AsposeCellsExamples.ChartMethodToImageWithStreamInt64Demo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamInt64Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
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

            // Create a memory stream to save the image
            using (MemoryStream imageStream = new MemoryStream())
            {
                try
                {
                    // Call ToImage with Stream and JPEG quality parameter (Int64)
                    chart.ToImage(imageStream, 90L);

                    // Save the stream to a file for demonstration
                    File.WriteAllBytes("ChartImage.jpg", imageStream.ToArray());
                    Console.WriteLine("Chart successfully converted to image with specified JPEG quality");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error converting chart to image: {ex.Message}");
                }
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

---

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

### Examples

```csharp
namespace AsposeCellsExamples.ChartMethodToImageWithStreamImageFormatDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Quarter");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(12000);
            worksheet.Cells["B3"].PutValue(15000);
            
            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Set chart data range
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            try
            {
                // Create a memory stream for the image
                using (MemoryStream imageStream = new MemoryStream())
                {
                    // Call the ToImage method with parameters (Stream, ImageType)
                    chart.ToImage(imageStream, ImageType.Png);
                    
                    // Save the stream to a file for demonstration
                    File.WriteAllBytes("ChartImage.png", imageStream.ToArray());
                    Console.WriteLine("Chart successfully exported to image stream.");
                }
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

---

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

### Examples

```csharp
namespace AsposeCellsExamples.ChartMethodToImageWithStreamImageTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for the chart
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
            chart.SetChartDataRange("A1:B4", true);
            
            // Create a memory stream to save the image
            using (MemoryStream imageStream = new MemoryStream())
            {
                try
                {
                    // Call the ToImage method with Stream and ImageType parameters
                    chart.ToImage(imageStream, ImageType.Png);
                    
                    Console.WriteLine("Chart successfully converted to image and saved to stream");
                    
                    // Here you would typically do something with the stream
                    // For example, save to a file:
                    File.WriteAllBytes("ChartImage.png", imageStream.ToArray());
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error converting chart to image: {ex.Message}");
                }
            }
            
            // Save the workbook
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### See Also

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

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

Saves to Tiff with 300 dpi and CCITT4 compression.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.TiffCompression = TiffCompression.CompressionCCITT4;

Workbook book = new Workbook(@"test.xls");
book.Worksheets[0].Charts[0].ToImage(@"chart.Tiff", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.TiffCompression = TiffCompression.CompressionCCITT4

Dim book As Workbook =  New Workbook("test.xls")
book.Worksheets(0).Charts(0).ToImage("chart.Tiff", options)

```

Saves to Jpeg with 300 dpi and 80 image quality.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.Quality = 80;

Workbook book = new Workbook(@"test.xls");
book.Worksheets[0].Charts[0].ToImage(@"chart.Jpeg", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions()
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.Quality = 80

Dim book As Workbook =  New Workbook("test.xls")
book.Worksheets(0).Charts(0).ToImage("chart.Jpeg", options)

```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

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

### Examples

```csharp
namespace AsposeCellsExamples.ChartMethodToImageWithStreamImageOrPrintOptionsDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Set chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Create image options
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.OnePagePerSheet = true;

            // Create a memory stream to save the image
            using (MemoryStream imageStream = new MemoryStream())
            {
                try
                {
                    // Call the ToImage method with Stream and ImageOrPrintOptions parameters
                    chart.ToImage(imageStream, options);

                    // Save the stream to a file for demonstration
                    File.WriteAllBytes("ChartImage.png", imageStream.ToArray());
                    Console.WriteLine("Chart successfully converted to image and saved.");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error converting chart to image: {ex.Message}");
                }
            }

            // Save the workbook
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


