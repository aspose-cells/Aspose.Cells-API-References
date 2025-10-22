##Aspose::Cells::Drawing::Shape::ToImage method
'Aspose::Cells::Drawing::Shape::ToImage method. Creates the shape image and saves it to a stream in the specified format in C++.'
## Shape::ToImage(Aspose::Cells::Drawing::ImageType) method
Creates the shape image and saves it to a stream in the specified format.
```cpp
Vector<uint8_t> Aspose::Cells::Drawing::Shape::ToImage(Aspose::Cells::Drawing::ImageType imageType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Aspose::Cells::Drawing::ImageType | The output stream. |
## Remarks
The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Enum [ImageType](../../imagetype/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::ToImage(const U16String\&, const ImageOrPrintOptions\&) method
Saves the shape to a file.
```cpp
void Aspose::Cells::Drawing::Shape::ToImage(const U16String &imageFile, const ImageOrPrintOptions &options)
```
## Examples
```cpp
U16String imgFile = u"exmaple.png";
ImageOrPrintOptions op;
shape.ToImage(imgFile, op);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::ToImage(const char16_t*, const ImageOrPrintOptions\&) method
Saves the shape to a file.
```cpp
void Aspose::Cells::Drawing::Shape::ToImage(const char16_t *imageFile, const ImageOrPrintOptions &options)
```
## Examples
```cpp
ImageOrPrintOptions op;
shape.ToImage(u"exmaple.png", op);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::ToImage(const ImageOrPrintOptions\&) method
Saves the shape to a stream.
```cpp
Vector<uint8_t> Aspose::Cells::Drawing::Shape::ToImage(const ImageOrPrintOptions &options)
```
## Examples
```cpp
ImageOrPrintOptions op;
Vector<uint8_t> imageStream = shape.ToImage(op);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
