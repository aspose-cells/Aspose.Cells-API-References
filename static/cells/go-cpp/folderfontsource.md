##FolderFontSource Class
'FolderFontSource class. Encapsulates the object that represents folderfontsource in Go.'
## FolderFontSource class
Represents the folder that contains TrueType font files.
```go
type FolderFontSource struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewFolderFontSource_String_Bool](./newfolderfontsource_string_bool/) | Ctor. |
|[NewFolderFontSource_FontSourceBase](./newfolderfontsource_fontsourcebase/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetFolderPath](./getfolderpath/) | Path to fonts folder. |
|[GetScanSubFolders](./getscansubfolders/) | Determines whether or not to scan the subfolders. |
|[GetType](./gettype/) | Returns the type of the font source. |
