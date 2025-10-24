##MemoryFontSource Class
'MemoryFontSource class. Encapsulates the object that represents memoryfontsource in Go.'
## MemoryFontSource class
Represents the single TrueType font file stored in memory.
```go
type MemoryFontSource struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewMemoryFontSource_Stream](./newmemoryfontsource_stream/) | Ctor. |
|[NewMemoryFontSource_FontSourceBase](./newmemoryfontsource_fontsourcebase/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetFontData](./getfontdata/) | Binary font data. |
|[GetType](./gettype/) | Returns the type of the font source. |
