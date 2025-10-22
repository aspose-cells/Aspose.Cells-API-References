##CellsColor Class
'CellsColor class. Encapsulates the object that represents cellscolor in Go.'
## CellsColor class
Represents all types of color.
```go
type CellsColor struct  {
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
|[IsShapeColor](./isshapecolor/) | Gets and set the color which should apply to cell or shape. |
|[SetIsShapeColor](./setisshapecolor/) | Gets and set the color which should apply to cell or shape. |
|[GetType](./gettype/) | The color type. |
|[GetThemeColor](./getthemecolor/) | Gets the theme color. Only applies for theme color type. |
|[SetThemeColor](./setthemecolor/) | Gets the theme color. Only applies for theme color type. |
|[GetColorIndex](./getcolorindex/) | Gets and sets the color index in the color palette. Only applies of indexed color. |
|[SetColorIndex](./setcolorindex/) | Gets and sets the color index in the color palette. Only applies of indexed color. |
|[GetColor](./getcolor/) | Gets and sets the RGB color. |
|[SetColor](./setcolor/) | Gets and sets the RGB color. |
|[GetArgb](./getargb/) | Gets and sets the color from a 32-bit ARGB value. |
|[SetArgb](./setargb/) | Gets and sets the color from a 32-bit ARGB value. |
|[GetTransparency](./gettransparency/) | Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTintOfShapeColor](./settintofshapecolor/) | Set the tint of the shape color |
