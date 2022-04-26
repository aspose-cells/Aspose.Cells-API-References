---
title: ToImage
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 590
url: /net/aspose.cells.charts/chart/toimage/
---
## Chart.ToImage method (1 of 5)

Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.

```csharp
public void ToImage(string imageFile)
```

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |

### Remarks

The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.

### See Also

* class [Chart](../../chart)
* namespace [Aspose.Cells.Charts](../../chart)
* assembly [Aspose.Cells](../../../)

---

## Chart.ToImage method (2 of 5)

Creates the chart image and saves it to a file in the Jpeg format.

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | String | The image file name with full path. |
| jpegQuality | Int64 | Jpeg quality. |

### Remarks

If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.

### See Also

* class [Chart](../../chart)
* namespace [Aspose.Cells.Charts](../../chart)
* assembly [Aspose.Cells](../../../)

---

## Chart.ToImage method (3 of 5)

Creates the chart image and saves it to a stream in the Jpeg format.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| jpegQuality | Int64 | Jpeg quality. |

### Remarks

If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.

### See Also

* class [Chart](../../chart)
* namespace [Aspose.Cells.Charts](../../chart)
* assembly [Aspose.Cells](../../../)

---

## Chart.ToImage method (4 of 5)

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

Workbook book = new Workbook(@"c:\test.xls");
book.Worksheets[0].Charts[0].ToImage(@"c:\chart.Tiff", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.TiffCompression = TiffCompression.CompressionCCITT4

Dim book As Workbook =  New Workbook("c:\test.xls")
book.Worksheets(0).Charts(0).ToImage("c:\chart.Tiff", options)

```

Saves to Jpeg with 300 dpi and 80 image quality.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.Quality = 80;

Workbook book = new Workbook(@"c:\test.xls");
book.Worksheets[0].Charts[0].ToImage(@"c:\chart.Jpeg", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions()
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.Quality = 80

Dim book As Workbook =  New Workbook("c:\test.xls")
book.Worksheets(0).Charts(0).ToImage("c:\chart.Jpeg", options)

```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* namespace [Aspose.Cells.Charts](../../chart)
* assembly [Aspose.Cells](../../../)

---

## Chart.ToImage method (5 of 5)

Creates the chart image and saves it to a stream in the specified format.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream. |
| options | ImageOrPrintOptions | Additional image creation options |

### Remarks

The format of the image is specified by using `options.ImageFormat`. The following formats are supported: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf.

If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* namespace [Aspose.Cells.Charts](../../chart)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
