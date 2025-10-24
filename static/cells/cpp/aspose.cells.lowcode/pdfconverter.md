##Aspose::Cells::LowCode::PdfConverter class
'Aspose::Cells::LowCode::PdfConverter class. Converter for converting template file to pdf in C++.'
## PdfConverter class
Converter for converting template file to pdf.
```cpp
class PdfConverter
```
## Methods
| Method | Description |
| --- | --- |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PdfConverter\& src)](./operator_asm/) | operator= |
| [PdfConverter(PdfConverter_Impl* impl)](./pdfconverter/) | Constructs from an implementation object. |
| [PdfConverter(const PdfConverter\& src)](./pdfconverter/) | Copy constructor. |
| static [Process(const U16String\& templateFile, const U16String\& resultFile)](./process/) | Converts given template file to pdf. |
| static [Process(const char16_t* templateFile, const char16_t* resultFile)](./process/) | Converts given template file to pdf. |
| static [Process(const LowCodeLoadOptions\& loadOptions, const LowCodeSaveOptions\& saveOptions)](./process/) | Converts template file to pdf. |
| [~PdfConverter()](./~pdfconverter/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
PdfConverter::Process(u"template.xlsx", u"res.pdf");
```
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
