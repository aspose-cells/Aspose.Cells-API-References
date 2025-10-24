##Aspose::Cells::Charts::Chart::ToImage method
'Aspose::Cells::Charts::Chart::ToImage method. Creates the chart image and saves it to a file. The extension of the file name determines the format of the image in C++.'
## Chart::ToImage(const U16String\&) method
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```cpp
void Aspose::Cells::Charts::Chart::ToImage(const U16String &imageFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | const U16String\& | The image file name with full path. |
## Remarks
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(const char16_t*) method
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```cpp
void Aspose::Cells::Charts::Chart::ToImage(const char16_t *imageFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | const char16_t* | The image file name with full path. |
## Remarks
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(const U16String\&, Aspose::Cells::Drawing::ImageType) method
Creates the chart image and saves it to a file in the specified image type.
```cpp
void Aspose::Cells::Charts::Chart::ToImage(const U16String &imageFile, Aspose::Cells::Drawing::ImageType imageType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | const U16String\& | The image file name with full path. |
| imageType | Aspose::Cells::Drawing::ImageType | The image type in which to save the image. |
## Remarks
The type of the image is specified by using **imageType**. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(const char16_t*, Aspose::Cells::Drawing::ImageType) method
Creates the chart image and saves it to a file in the specified image type.
```cpp
void Aspose::Cells::Charts::Chart::ToImage(const char16_t *imageFile, Aspose::Cells::Drawing::ImageType imageType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | const char16_t* | The image file name with full path. |
| imageType | Aspose::Cells::Drawing::ImageType | The image type in which to save the image. |
## Remarks
The type of the image is specified by using **imageType**. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(const U16String\&, int64_t) method
Creates the chart image and saves it to a file in the Jpeg format.
>Deprecated
>
>Use Chart.ToImage(string,ImageOrPrintOptions) method instead.
```cpp
void Aspose::Cells::Charts::Chart::ToImage(const U16String &imageFile, int64_t jpegQuality)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | const U16String\& | The image file name with full path. |
| jpegQuality | int64_t | Jpeg quality. |
## Remarks
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing. NOTE: This method is now obsolete. Instead, please use ToImage(string,ImageOrPrintOptions) method with specified quality. This method will be removed 12 months later since March 2025. **Aspose** apologizes for any inconvenience you may have experienced.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(const char16_t*, int64_t) method
Creates the chart image and saves it to a file in the Jpeg format.
>Deprecated
>
>Use Chart.ToImage(string,ImageOrPrintOptions) method instead.
```cpp
void Aspose::Cells::Charts::Chart::ToImage(const char16_t *imageFile, int64_t jpegQuality)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | const char16_t* | The image file name with full path. |
| jpegQuality | int64_t | Jpeg quality. |
## Remarks
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing. NOTE: This method is now obsolete. Instead, please use ToImage(string,ImageOrPrintOptions) method with specified quality. This method will be removed 12 months later since March 2025. **Aspose** apologizes for any inconvenience you may have experienced.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(int64_t) method
Creates the chart image and saves it to a stream in the Jpeg format.
```cpp
Vector<uint8_t> Aspose::Cells::Charts::Chart::ToImage(int64_t jpegQuality)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | int64_t | The output stream. |
## Remarks
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(Aspose::Cells::Drawing::ImageType) method
Creates the chart image and saves it to a stream in the specified format.
```cpp
Vector<uint8_t> Aspose::Cells::Charts::Chart::ToImage(Aspose::Cells::Drawing::ImageType imageType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Aspose::Cells::Drawing::ImageType | The output stream. |
## Remarks
The type of the image is specified by using **imageType**. The following types are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(const U16String\&, const ImageOrPrintOptions\&) method
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```cpp
void Aspose::Cells::Charts::Chart::ToImage(const U16String &imageFile, const ImageOrPrintOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | const U16String\& | The image file name with full path. |
| options | const ImageOrPrintOptions\& | Additional image creation options |
## Remarks
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.
## Examples
```cpp
Aspose::Cells::Startup();
//Saves to Tiff with 300 dpi and CCITT4 compression.
ImageOrPrintOptions opt;
opt.SetHorizontalResolution(300);
opt.SetVerticalResolution(300);
opt.SetTiffCompression(TiffCompression::CompressionCCITT4);
Workbook book(u"test.xls");
book.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(u"chart.Tiff", opt);
//Saves to Jpeg with 300 dpi and 80 image quality.
ImageOrPrintOptions options2;
options2.SetHorizontalResolution(300);
options2.SetVerticalResolution(300);
options2.SetQuality(80);
U16String val = u"chart.Jpeg";
Workbook book2(u"test.xls");
book2.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(val, opt);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(const char16_t*, const ImageOrPrintOptions\&) method
Creates the chart image and saves it to a file. The extension of the file name determines the format of the image.
```cpp
void Aspose::Cells::Charts::Chart::ToImage(const char16_t *imageFile, const ImageOrPrintOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | const char16_t* | The image file name with full path. |
| options | const ImageOrPrintOptions\& | Additional image creation options |
## Remarks
The format of the image is specified by using the extension of the file name. For example, if you specify "myfile.png", then the image will be saved in the PNG format. The following file extensions are recognized: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.
## Examples
```cpp
Aspose::Cells::Startup();
//Saves to Tiff with 300 dpi and CCITT4 compression.
ImageOrPrintOptions opt;
opt.SetHorizontalResolution(300);
opt.SetVerticalResolution(300);
opt.SetTiffCompression(TiffCompression::CompressionCCITT4);
Workbook book(u"test.xls");
book.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(u"chart.Tiff", opt);
//Saves to Jpeg with 300 dpi and 80 image quality.
ImageOrPrintOptions options2;
options2.SetHorizontalResolution(300);
options2.SetVerticalResolution(300);
options2.SetQuality(80);
Workbook book2(u"test.xls");
book2.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(u"chart.Jpeg", opt);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## Chart::ToImage(const ImageOrPrintOptions\&) method
Creates the chart image and saves it to a stream in the specified format.
```cpp
Vector<uint8_t> Aspose::Cells::Charts::Chart::ToImage(const ImageOrPrintOptions &options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | const ImageOrPrintOptions\& | The output stream. |
## Remarks
The type of the image is specified by using **options.ImageType**. The following formats are supported: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.
If the width or height is zero or the chart is not supported according to Supported [Charts](../../) List, this method will do nothing. Please refer to [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) for more details.
## Examples
```cpp
Aspose::Cells::Startup();
//Gets a bitmap object with 200 x dpi and 300 y dpi.
ImageOrPrintOptions opt;
opt.SetHorizontalResolution(200);
opt.SetVerticalResolution(300);
Workbook book(u"test.xls");
Vector<uint8_t> chartObject = book.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(opt);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
