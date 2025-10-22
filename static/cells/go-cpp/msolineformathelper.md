##MsoLineFormatHelper Class
'MsoLineFormatHelper class. Encapsulates the object that represents msolineformathelper in Go.'
## MsoLineFormatHelper class
Represents line and arrowhead formatting.
```go
type MsoLineFormatHelper struct  {
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
|[IsVisible](./isvisible/) | Indicates whether the object is visible. |
|[SetIsVisible](./setisvisible/) | Indicates whether the object is visible. |
|[GetStyle](./getstyle/) | Returns a Style object that represents the style of the specified range. |
|[SetStyle](./setstyle/) | Returns a Style object that represents the style of the specified range. |
|[GetForeColor](./getforecolor/) | Gets and sets the border line fore color. |
|[SetForeColor](./setforecolor/) | Gets and sets the border line fore color. |
|[GetBackColor](./getbackcolor/) | Gets and sets the border line back color. |
|[SetBackColor](./setbackcolor/) | Gets and sets the border line back color. |
|[GetDashStyle](./getdashstyle/) | Gets or sets the dash style for the specified line. |
|[SetDashStyle](./setdashstyle/) | Gets or sets the dash style for the specified line. |
|[GetTransparency](./gettransparency/) | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
|[GetWeight](./getweight/) | Returns or sets the weight of the line ,in units of pt. |
|[SetWeight](./setweight/) | Returns or sets the weight of the line ,in units of pt. |
