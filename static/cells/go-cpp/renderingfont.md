##RenderingFont Class
'RenderingFont class. Encapsulates the object that represents renderingfont in Go.'
## RenderingFont class
Font for rendering.
```go
type RenderingFont struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRenderingFont](./newrenderingfont/) | Initializes a new instance of the RenderingFont |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetName](./getname/) | Gets name of the font. |
|[GetSize](./getsize/) | Gets size of the font in points. |
|[GetBold](./getbold/) | Gets or sets bold for the font. |
|[SetBold](./setbold/) | Gets or sets bold for the font. |
|[GetItalic](./getitalic/) | Gets or sets italic for the font. |
|[SetItalic](./setitalic/) | Gets or sets italic for the font. |
|[GetColor](./getcolor/) | Gets or sets color for the font. |
|[SetColor](./setcolor/) | Gets or sets color for the font. |
