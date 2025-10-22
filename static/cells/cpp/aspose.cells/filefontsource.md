##Aspose::Cells::FileFontSource class
'Aspose::Cells::FileFontSource class. Represents the single TrueType font file stored in the file system in C++.'
## FileFontSource class
Represents the single TrueType font file stored in the file system.
```cpp
class FileFontSource : public Aspose::Cells::FontSourceBase
```
## Methods
| Method | Description |
| --- | --- |
| explicit [FileFontSource(const U16String\& filePath)](./filefontsource/) | Ctor. |
| explicit [FileFontSource(const char16_t* filePath)](./filefontsource/) | Ctor. |
| [FileFontSource(FileFontSource_Impl* impl)](./filefontsource/) | Constructs from an implementation object. |
| [FileFontSource(const FileFontSource\& src)](./filefontsource/) | Copy constructor. |
| [FileFontSource(const FontSourceBase\& src)](./filefontsource/) | Constructs from a parent object. |
| [FontSourceBase(FontSourceBase_Impl* impl)](../fontsourcebase/fontsourcebase/) | Constructs from an implementation object. |
| [FontSourceBase(const FontSourceBase\& src)](../fontsourcebase/fontsourcebase/) | Copy constructor. |
| [GetFilePath()](./getfilepath/) | Path to font file. |
| virtual [GetType()](./gettype/) | Returns the type of the font source. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FileFontSource\& src)](./operator_asm/) | operator= |
| [operator=(const FontSourceBase\& src)](../fontsourcebase/operator_asm/) | operator= |
| [~FileFontSource()](./~filefontsource/) | Destructor. |
| [~FontSourceBase()](../fontsourcebase/~fontsourcebase/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [FontSourceBase](../fontsourcebase/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
