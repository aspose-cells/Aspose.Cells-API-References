##FileFontSource Class
'FileFontSource class. Encapsulates the object that represents filefontsource in Go.'
## FileFontSource class
Represents the single TrueType font file stored in the file system.
```go
type FileFontSource struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewFileFontSource_String](./newfilefontsource_string/) | Ctor. |
|[NewFileFontSource_FontSourceBase](./newfilefontsource_fontsourcebase/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetFilePath](./getfilepath/) | Path to font file. |
|[GetType](./gettype/) | Returns the type of the font source. |
