##Border Class
'Border class. Encapsulates the object that represents border in Go.'
## Border class
Encapsulates the object that represents the cell border.
```go
type Border struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetThemeColor](./getthemecolor/) | Gets and sets the theme color of the border. |
|[SetThemeColor](./setthemecolor/) | Gets and sets the theme color of the border. |
|[GetColor](./getcolor/) | Gets or sets the Color of the border. |
|[SetColor](./setcolor/) | Gets or sets the Color of the border. |
|[GetArgbColor](./getargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
|[SetArgbColor](./setargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
|[GetLineStyle](./getlinestyle/) | Gets or sets the cell border type. |
|[SetLineStyle](./setlinestyle/) | Gets or sets the cell border type. |
