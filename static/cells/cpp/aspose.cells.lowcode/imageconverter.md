##Aspose::Cells::LowCode::ImageConverter class
'Aspose::Cells::LowCode::ImageConverter class. Converter for converting template file to images in C++.'
## ImageConverter class
Converter for converting template file to images.
```cpp
class ImageConverter
```
## Methods
| Method | Description |
| --- | --- |
| [ImageConverter(ImageConverter_Impl* impl)](./imageconverter/) | Constructs from an implementation object. |
| [ImageConverter(const ImageConverter\& src)](./imageconverter/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ImageConverter\& src)](./operator_asm/) | operator= |
| static [Process(const U16String\& templateFile, const U16String\& resultFile)](./process/) | Converts template file to images. |
| static [Process(const char16_t* templateFile, const char16_t* resultFile)](./process/) | Converts template file to images. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions)](./process/) | Converts template file to images. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions, const AbstractLowCodeSaveOptionsProvider\& provider)](./process/) | Converts template file to images. |
| [~ImageConverter()](./~imageconverter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
ImageConverter::Process(u"template.xlsx", u"res.png");
```
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
