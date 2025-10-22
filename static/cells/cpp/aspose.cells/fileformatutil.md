##Aspose::Cells::FileFormatUtil class
'Aspose::Cells::FileFormatUtil class. Provides utility methods for converting file format enums to strings or file extensions and back in C++.'
## FileFormatUtil class
Provides utility methods for converting file format enums to strings or file extensions and back.
```cpp
class FileFormatUtil
```
## Methods
| Method | Description |
| --- | --- |
| static [DetectFileFormat(const Vector \<uint8_t\>\& stream)](./detectfileformat/) | Detects and returns the information about a format of an excel stored in a stream. |
| static [DetectFileFormat(const Vector \<uint8_t\>\& stream, const U16String\& password)](./detectfileformat/) | Detects and returns the information about a format of an excel stored in a stream. |
| static [DetectFileFormat(const Vector \<uint8_t\>\& stream, const char16_t* password)](./detectfileformat/) | Detects and returns the information about a format of an excel stored in a stream. |
| static [DetectFileFormat(const U16String\& filePath)](./detectfileformat/) | Detects and returns the information about a format of an excel stored in a file. |
| static [DetectFileFormat(const char16_t* filePath)](./detectfileformat/) | Detects and returns the information about a format of an excel stored in a file. |
| static [DetectFileFormat(const U16String\& filePath, const U16String\& password)](./detectfileformat/) | Detects and returns the information about a format of an excel stored in a file. |
| static [DetectFileFormat(const char16_t* filePath, const char16_t* password)](./detectfileformat/) | Detects and returns the information about a format of an excel stored in a file. |
| static [ExtensionToSaveFormat(const U16String\& extension)](./extensiontosaveformat/) | Converts a file name extension into a SaveFormat value. |
| static [ExtensionToSaveFormat(const char16_t* extension)](./extensiontosaveformat/) | Converts a file name extension into a SaveFormat value. |
| static [FileFormatToSaveFormat(FileFormatType format)](./fileformattosaveformat/) | Converting file format to save format. |
| static [IsTemplateFormat(const U16String\& extension)](./istemplateformat/) | Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
| static [IsTemplateFormat(const char16_t* extension)](./istemplateformat/) | Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
| static [LoadFormatToExtension(LoadFormat loadFormat)](./loadformattoextension/) | Converts a load format enumerated value into a file extension. |
| static [LoadFormatToSaveFormat(LoadFormat loadFormat)](./loadformattosaveformat/) | Converts a LoadFormat value to a SaveFormat value if possible. |
| static [SaveFormatToExtension(SaveFormat format)](./saveformattoextension/) | Converts a save format enumerated value into a file extension. |
| static [SaveFormatToLoadFormat(SaveFormat saveFormat)](./saveformattoloadformat/) | Converts a SaveFormat value to a LoadFormat value if possible. |
| static [VerifyPassword(const Vector \<uint8_t\>\& stream, const U16String\& password)](./verifypassword/) | Detects and returns the information about a format of an excel stored in a stream. |
| static [VerifyPassword(const Vector \<uint8_t\>\& stream, const char16_t* password)](./verifypassword/) | Detects and returns the information about a format of an excel stored in a stream. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
