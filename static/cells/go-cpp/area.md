##Area Class
'Area class. Encapsulates the object that represents area in Go.'
## Area class
Encapsulates the object that represents an area format.
```go
type Area struct  {
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
|[GetBackgroundColor](./getbackgroundcolor/) | Gets or sets the background Color of the Area. |
|[SetBackgroundColor](./setbackgroundcolor/) | Gets or sets the background Color of the Area. |
|[GetForegroundColor](./getforegroundcolor/) | Gets or sets the foreground Color. |
|[SetForegroundColor](./setforegroundcolor/) | Gets or sets the foreground Color. |
|[GetFormatting](./getformatting/) | Represents the formatting of the area. |
|[SetFormatting](./setformatting/) | Represents the formatting of the area. |
|[GetInvertIfNegative](./getinvertifnegative/) | If the property is true and the value of chart point is a negative number,the foreground color and background color will be exchanged. |
|[SetInvertIfNegative](./setinvertifnegative/) | If the property is true and the value of chart point is a negative number,the foreground color and background color will be exchanged. |
|[GetFillFormat](./getfillformat/) | Represents a FillFormat object that contains fill formatting properties for the specified chart or shape. |
|[GetTransparency](./gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
