---
title: to_image方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 120
url: /zh/python-net/aspose.cells.charts/chart/to_image/
is_root: false
---
##  to_image(image_file) {#str}
创建图表图像并将其保存到文件中。
文件名的扩展名决定了图像的格式。



```python
def to_image(self, image_file):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| image_file | str |带完整路径的图像文件名。|
### 评论

图像的格式通过使用文件名的扩展名来指定。
例如，如果您指定“myfile.png”，那么图像将被保存
采用 PNG 格式。可识别以下文件扩展名：
.bmp、.gif、.png、.jpg、.jpeg、.tiff、.tif、.emf。


如果宽度或高度为零或根据支持的图表列表不支持图表，则此方法将不执行任何操作。

##  to_image(image_file, image_type) {#str-aspose.cells.drawing.ImageType}
创建图表图像并将其保存到指定图像类型的文件中。



```python
def to_image(self, image_file, image_type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| image_file | str |带完整路径的图像文件名。|
| image_type | aspose.cells.drawing.ImageType |保存图像的图像类型。|
### 评论

图像的类型使用 `imageType` 指定。
支持以下类型：
ImageType.Bmp、ImageType.Gif、ImageType.Png、ImageType.Jpeg、ImageType.Tiff、ImageType.Emf。


如果宽度或高度为零或根据支持的图表列表不支持图表，则此方法将不执行任何操作。

##  to_image(image_file, jpeg_quality) {#str-int}
创建图表图像并将其保存到 Jpeg 格式的文件中。



```python
def to_image(self, image_file, jpeg_quality):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| image_file | str |带完整路径的图像文件名。|
| jpeg_quality | int | Jpeg 质量。|
### 评论

如果宽度或高度为零或根据支持的图表列表不支持图表，则此方法将不执行任何操作。

##  to_image(stream, jpeg_quality) {#io.RawIOBase-int}

创建图表图像并将其保存到 Jpeg 格式的流中。



```python
def to_image(self, stream, jpeg_quality):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |输出流。|
| jpeg_quality | int | Jpeg 质量。|
### 评论

如果宽度或高度为零或根据支持的图表列表不支持图表，则此方法将不执行任何操作。

##  to_image(stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}

创建图表图像并将其保存到指定格式的流中。



```python
def to_image(self, stream, image_type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |输出流。|
| image_type | aspose.cells.drawing.ImageType |保存图像的图像类型。|
### 评论

图像的类型使用 `imageType` 指定。
支持以下类型：
ImageType.Bmp、ImageType.Gif、ImageType.Png、ImageType.Jpeg、ImageType.Tiff、ImageType.Emf。


如果宽度或高度为零或根据支持的图表列表不支持图表，则此方法将不执行任何操作。

##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
创建图表图像并将其保存到文件中。
文件名的扩展名决定了图像的格式。



```python
def to_image(self, image_file, options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| image_file | str |带完整路径的图像文件名。|
| options | aspose.cells.rendering.ImageOrPrintOptions |其他图像创建选项|
### 评论

图像的格式通过使用文件名的扩展名来指定。
例如，如果您指定“myfile.png”，那么图像将被保存
采用 PNG 格式。可识别以下文件扩展名：
.bmp、.gif、.png、.jpg、.jpeg、.tiff、.tif、.emf。


如果宽度或高度为零或根据支持的图表列表不支持图表，则此方法将不执行任何操作。
请参阅[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)更多细节。
### 例子

使用 300 dpi 和 CCITT4 压缩保存为 Tiff。

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, TiffCompression

options = ImageOrPrintOptions()
options.horizontal_resolution = 300
options.vertical_resolution = 300
options.tiff_compression = TiffCompression.COMPRESSION_CCITT4
book = Workbook(r"test.xls")
book.worksheets[0].charts[0].to_image(r"chart.Tiff", options)

```


以 300 dpi 和 80 图像质量保存为 Jpeg。

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions

options = ImageOrPrintOptions()
options.horizontal_resolution = 300
options.vertical_resolution = 300
options.quality = 80
book = Workbook(r"test.xls")
book.worksheets[0].charts[0].to_image(r"chart.Jpeg", options)

```


##  to_image(stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}
创建图表图像并将其保存到指定格式的流中。



```python
def to_image(self, stream, options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |输出流。|
| options | aspose.cells.rendering.ImageOrPrintOptions |其他图像创建选项|
### 评论

图像的类型使用 `options.ImageType` 指定。
支持以下格式：
ImageType.Bmp、ImageType.Gif、ImageType.Png、ImageType.Jpeg、ImageType.Tiff、ImageType.Emf。


如果宽度或高度为零或根据支持的图表列表不支持图表，则此方法将不执行任何操作。
请参阅[支持的图表列表](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)更多细节。


### 也可以看看
* 模块 [aspose.cells.charts](../../)
* 类 [Chart](/cells/zh/python-net/aspose.cells.charts/chart)
