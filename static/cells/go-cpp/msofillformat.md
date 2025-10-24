##MsoFillFormat Class
'MsoFillFormat class. Encapsulates the object that represents msofillformat in Go.'
## MsoFillFormat class
Represents fill formatting for a shape.
```go
type MsoFillFormat struct  {
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
|[GetForeColor](./getforecolor/) | Gets and sets the fill fore color. |
|[SetForeColor](./setforecolor/) | Gets and sets the fill fore color. |
|[GetTransparency](./gettransparency/) | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
|[GetBackColor](./getbackcolor/) | Gets and sets the file back color. |
|[SetBackColor](./setbackcolor/) | Gets and sets the file back color. |
|[GetImageData](./getimagedata/) | Gets and sets the Texture and Picture fill data. |
|[SetImageData](./setimagedata/) | Gets and sets the Texture and Picture fill data. |
|[SetOneColorGradient](./setonecolorgradient/) | Sets the specified fill to a one-color gradient. |
|[GetTexture](./gettexture/) | Gets the texture fill type. |
|[IsVisible](./isvisible/) | Indicates whether there is fill. |
|[SetIsVisible](./setisvisible/) | Indicates whether there is fill. |
