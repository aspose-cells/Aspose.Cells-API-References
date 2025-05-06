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
// Called: System.Drawing.Bitmap bitmap = workbook.Worksheets[0].Charts[0].ToImage();
[Test]
        public void Method_ToImage()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Logins.xlsx&quot;);
#if !NETCOREAPP2_0
            System.Drawing.Bitmap bitmap = workbook.Worksheets[0].Charts[0].ToImage();
            bitmap.Save(Constants.destPath + &quot;Charts2Image/Test_143987.jpg&quot;, ImageFormat.Jpeg);
#endif
            workbook.Save(Constants.destPath + &quot;Logins.xlsx&quot;);
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
// Called: chart.ToImage(Constants.destPath + &amp;quot;Charts/BoxWhisker/Chart&amp;quot; + chart.Name + &amp;quot;.png&amp;quot;);
[Test]
        public void Method_String_()
        {
            // for show inner/outlier points and datalabels
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts/BoxWhisker/MyTest.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[&quot;Sheet2&quot;];
            foreach (Chart chart in worksheet.Charts)
            {
                chart.ToImage(Constants.destPath + &quot;Charts/BoxWhisker/Chart&quot; + chart.Name + &quot;.png&quot;);
            }
            return;
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
[Test]
        public void Method_ImageType_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43750_&quot;;

            Aspose.Cells.LoadOptions loadOptions = new Aspose.Cells.LoadOptions(LoadFormat.Xlsx);
            Workbook workbook = new Workbook(filePath + &quot;Template.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[1];
            workbook.CalculateFormula();
            foreach (PivotTable pivotTable in workbook.Worksheets[2].PivotTables)
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + &quot;NET43750.xlsx&quot;);
            int index = 0;
            foreach (Chart chart in workbook.Worksheets[0].Charts)
            {
                chart.RefreshPivotData();
#if !NETCOREAPP2_0
                chart.ToImage(Constants.PIVOT_CHECK_FILE_PATH
                    + &quot;NET43750_out_&quot; + index.ToString() + &quot;.png&quot;, ImageType.Png);
#else 
                chart.ToImage(Constants.PIVOT_CHECK_FILE_PATH + &quot;NET43750_out_&quot; + index.ToString() + &quot;.bmp&quot;);
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

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


