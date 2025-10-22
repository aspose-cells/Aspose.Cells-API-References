##GlowEffect Class
'GlowEffect class. Encapsulates the object that represents gloweffect in Go.'
## GlowEffect class
This class specifies a glow effect, in which a color blurred outlineis added outside the edges of the object.
```go
type GlowEffect struct  {
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
|[GetColor](./getcolor/) | Gets the color of the glow effect. |
|[SetColor](./setcolor/) | Gets the color of the glow effect. |
|[GetSize](./getsize/) | Gets and sets the radius of the glow, in unit of points. |
|[SetSize](./setsize/) | Gets and sets the radius of the glow, in unit of points. |
|[GetTransparency](./gettransparency/) | Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear). |
|[SetTransparency](./settransparency/) | Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear). |
