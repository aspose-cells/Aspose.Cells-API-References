##to_image method
## to_image(self, image_file) {#System.String}
Creates the chart image and saves it to a file.
The extension of the file name determines the format of the image.
```python
def to_image(self, image_file):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| image_file | System.String | The image file name with full path. |
### Remarks
The format of the image is specified by using the extension of the file name.
For example, if you specify "myfile.png", then the image will be saved
in the PNG format. The following file extensions are recognized:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
## to_image(self, image_file, image_type) {#System.String-aspose.cells.drawing.ImageType}
Creates the chart image and saves it to a file in the specified image type.
```python
def to_image(self, image_file, image_type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| image_file | System.String | The image file name with full path. |
| image_type | aspose.cells.drawing.ImageType | The image type in which to save the image. |
### Remarks
The type of the image is specified by using `imageType`.
The following types are supported:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
## to_image(self, image_file, jpeg_quality) {#System.String-int}
Creates the chart image and saves it to a file in the Jpeg format.
```python
def to_image(self, image_file, jpeg_quality):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| image_file | System.String | The image file name with full path. |
| jpeg_quality | int | Jpeg quality. |
### Remarks
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
NOTE: This method is now obsolete. Instead,
please use ToImage(string,ImageOrPrintOptions) method with specified quality.
This method will be removed 12 months later since March 2025.
Aspose apologizes for any inconvenience you may have experienced.
## to_image(self, stream, jpeg_quality) {#io.RawIOBase-int}
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
## to_image(self, stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}
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
## to_image(self, image_file, options) {#System.String-aspose.cells.rendering.ImageOrPrintOptions}
Creates the chart image and saves it to a file.
The extension of the file name determines the format of the image.
```python
def to_image(self, image_file, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| image_file | System.String | The image file name with full path. |
| options | aspose.cells.rendering.ImageOrPrintOptions | Additional image creation options |
### Remarks
The format of the image is specified by using the extension of the file name.
For example, if you specify "myfile.png", then the image will be saved
in the PNG format. The following file extensions are recognized:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing.
Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.
### Example
Saves to Tiff with 300 dpi and CCITT4 compression.
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
Saves to Jpeg with 300 dpi and 80 image quality.
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
## to_image(self, stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}
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
* module [`aspose.cells.charts`](../../)
* class [`Chart`](/cells/python-net/aspose.cells.charts/chart)
