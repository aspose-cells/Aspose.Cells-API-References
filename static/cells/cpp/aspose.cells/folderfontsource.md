##Aspose::Cells::FolderFontSource class
'Aspose::Cells::FolderFontSource class. Represents the folder that contains TrueType font files in C++.'
## FolderFontSource class
Represents the folder that contains TrueType font files.
```cpp
class FolderFontSource : public Aspose::Cells::FontSourceBase
```
## Methods
| Method | Description |
| --- | --- |
| [FolderFontSource(const U16String\& folderPath, bool scanSubfolders)](./folderfontsource/) | Ctor. |
| [FolderFontSource(const char16_t* folderPath, bool scanSubfolders)](./folderfontsource/) | Ctor. |
| [FolderFontSource(FolderFontSource_Impl* impl)](./folderfontsource/) | Constructs from an implementation object. |
| [FolderFontSource(const FolderFontSource\& src)](./folderfontsource/) | Copy constructor. |
| [FolderFontSource(const FontSourceBase\& src)](./folderfontsource/) | Constructs from a parent object. |
| [FontSourceBase(FontSourceBase_Impl* impl)](../fontsourcebase/fontsourcebase/) | Constructs from an implementation object. |
| [FontSourceBase(const FontSourceBase\& src)](../fontsourcebase/fontsourcebase/) | Copy constructor. |
| [GetFolderPath()](./getfolderpath/) | Path to fonts folder. |
| [GetScanSubFolders()](./getscansubfolders/) | Determines whether or not to scan the subfolders. |
| virtual [GetType()](./gettype/) | Returns the type of the font source. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FolderFontSource\& src)](./operator_asm/) | operator= |
| [operator=(const FontSourceBase\& src)](../fontsourcebase/operator_asm/) | operator= |
| [~FolderFontSource()](./~folderfontsource/) | Destructor. |
| [~FontSourceBase()](../fontsourcebase/~fontsourcebase/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [FontSourceBase](../fontsourcebase/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
