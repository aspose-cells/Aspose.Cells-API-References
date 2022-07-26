---
title: ToImage
second_title: Aspose.Cells for .NET API 参考
description: 获取 32 位位图图表对象.
type: docs
weight: 590
url: /zh/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

获取 32 位`位图`图表对象.

```csharp
public Bitmap ToImage()
```

### 返回值

图表的图片。

### 评论

如果宽度或高度为零或根据支持的图表列表不支持图表，它将返回null。 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 也可以看看

* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

获取 32 位`位图`图表对象. `ImageOrPrintOptions.ImageFormat` , ImageOrPrintOptions.TiffCompression 和 ImageOrPrintOptions.Quality 属性被忽略。

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| options | ImageOrPrintOptions | 其他图像创建选项 |

### 返回值

图表的图片。

### 评论

返回一个 32 位的位图对象，因此 ImageOrPrintOptions.ImageFormat、ImageOrPrintOptions.TiffCompression 和 ImageOrPrintOptions.Quality 属性不会影响方法。 如果宽度或高度为零或根据支持的图表列表不支持图表，则将返回 null. 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 例子

获取 200 x dpi 和 300 y dpi 的位图对象。

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

### 也可以看看

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

创建图表图像并将其保存到文件中。 文件名的扩展名决定图像的格式。

```csharp
public void ToImage(string imageFile)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | String | 带有完整路径的图像文件名。 |

### 评论

使用文件名的扩展名指定图像的格式。 例如，如果指定“myfile.png”，则图像将保存为PNG格式的 。可识别以下文件扩展名： .bmp、.gif、.png、.jpg、.jpeg、.tiff、.tif、.emf。

如果宽度或高度为零或根据支持的图表列表不支持图表，此方法将不起作用。 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 也可以看看

* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

创建图表图像并将其保存到指定图像类型的文件中。

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | String | 带有完整路径的图像文件名。 |
| imageType | ImageType | 保存图像的图像类型。 |

### 评论

图像的类型通过使用指定`图像类型`. 支持以下类型： ImageType.Bmp、ImageType.Gif、ImageType.Png、ImageType.Jpeg、ImageType.Tiff、ImageType.Emf。

如果宽度或高度为零或根据支持的图表列表不支持图表，此方法将不起作用。 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 也可以看看

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

创建图表图像并将其保存到 Jpeg 格式的文件中。

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | String | 带有完整路径的图像文件名。 |
| jpegQuality | Int64 | Jpeg 质量。 |

### 评论

如果宽度或高度为零或根据支持的图表列表不支持图表，此方法将不起作用。 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 也可以看看

* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

创建图表图像并将其保存到 Jpeg 格式的流中。

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 输出流。 |
| jpegQuality | Int64 | Jpeg 质量。 |

### 评论

如果宽度或高度为零或根据支持的图表列表不支持图表，此方法将不起作用。 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 也可以看看

* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

创建图表图像并将其保存到指定格式的流中。

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 输出流。 |
| imageType | ImageType | 保存图像的图像类型。 |

### 评论

图像的类型通过使用指定`图像类型`. 支持以下类型： ImageType.Bmp、ImageType.Gif、ImageType.Png、ImageType.Jpeg、ImageType.Tiff、ImageType.Emf。

如果宽度或高度为零或根据支持的图表列表不支持图表，此方法将不起作用。 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 也可以看看

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

创建图表图像并将其保存到文件中。 文件名的扩展名决定图像的格式。

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| imageFile | String | 带有完整路径的图像文件名。 |
| options | ImageOrPrintOptions | 其他图像创建选项 |

### 评论

使用文件名的扩展名指定图像的格式。 例如，如果指定“myfile.png”，则图像将保存为PNG格式的 。可识别以下文件扩展名： .bmp、.gif、.png、.jpg、.jpeg、.tiff、.tif、.emf。

如果宽度或高度为零或根据支持的图表列表不支持图表，此方法将不起作用。 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 例子

以 300 dpi 和 CCITT4 压缩保存到 Tiff。 以 300 dpi 和 80 图像质量保存为 Jpeg。

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

### 也可以看看

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

创建图表图像并将其保存到指定格式的流中。

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 输出流。 |
| options | ImageOrPrintOptions | 其他图像创建选项 |

### 评论

图像的类型通过使用指定`options.ImageType`. 支持以下格式： ImageType.Bmp、ImageType.Gif、ImageType.Png、ImageType.Jpeg、ImageType.Tiff、ImageType.Emf。

如果宽度或高度为零或根据支持的图表列表不支持图表，此方法将不起作用。 请参考[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)了解更多详情。

### 也可以看看

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* 命名空间 [Aspose.Cells.Charts](../../chart)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
