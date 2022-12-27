---
title: to_image method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 120
url: /python-net/aspose.cells.charts/chart/to_image/
is_root: false
---

## to_image(image_file) {#str}

Creates the chart image and saves it to a file.
The extension of the file name determines the format of the image.



```python
def to_image(self, image_file):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_file | str | The image file name with full path. |
### Remarks

The format of the image is specified by using the extension of the file name.
For example, if you specify "myfile.png", then the image will be saved
in the PNG format. The following file extensions are recognized: 
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

## to_image(image_file, image_type) {#str-aspose.cells.drawing.ImageType}

Creates the chart image and saves it to a file in the specified image type.



```python
def to_image(self, image_file, image_type):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_file | str | The image file name with full path. |
| image_type | aspose.cells.drawing.ImageType | The image type in which to save the image. |
### Remarks

The type of the image is specified by using `imageType`.
The following types are supported: 
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

## to_image(image_file, jpeg_quality) {#str-int}

Creates the chart image and saves it to a file in the Jpeg format.



```python
def to_image(self, image_file, jpeg_quality):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_file | str | The image file name with full path. |
| jpeg_quality | int | Jpeg quality. |
### Remarks

If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

## to_image(stream, jpeg_quality) {#io.RawIOBase-int}

Creates the chart image and saves it to a stream in the Jpeg format.



```python
def to_image(self, stream, jpeg_quality):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The output stream. |
| jpeg_quality | int | Jpeg quality. |
### Remarks

If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

## to_image(stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}

Creates the chart image and saves it to a stream in the specified format.



```python
def to_image(self, stream, image_type):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The output stream. |
| image_type | aspose.cells.drawing.ImageType | The image type in which to save the image. |
### Remarks

The type of the image is specified by using `imageType`.
The following types are supported: 
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.

## to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}

Creates the chart image and saves it to a file.
The extension of the file name determines the format of the image.



```python
def to_image(self, image_file, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| image_file | str | The image file name with full path. |
| options | aspose.cells.rendering.ImageOrPrintOptions | Additional image creation options |
### Remarks

The format of the image is specified by using the extension of the file name.
For example, if you specify "myfile.png", then the image will be saved
in the PNG format. The following file extensions are recognized: 
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.

## to_image(stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}

Creates the chart image and saves it to a stream in the specified format.



```python
def to_image(self, stream, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The output stream. |
| options | aspose.cells.rendering.ImageOrPrintOptions | Additional image creation options |
### Remarks

The type of the image is specified by using `options.ImageType`.
The following formats are supported: 
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.


### See Also
* module [aspose.cells.charts](../../)
* class [Chart](/cells/python-net/aspose.cells.charts/chart)
