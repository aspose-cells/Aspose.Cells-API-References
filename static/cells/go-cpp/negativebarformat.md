##NegativeBarFormat Class
'NegativeBarFormat class. Encapsulates the object that represents negativebarformat in Go.'
## NegativeBarFormat class
Represents the color settings of the data bars for negative values that are defined by a data bar conditional formatting rule.
```go
type NegativeBarFormat struct  {
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
|[GetBorderColor](./getbordercolor/) | Gets or sets a FormatColor object that you can use to specify the border color for negative data bars. |
|[SetBorderColor](./setbordercolor/) | Gets or sets a FormatColor object that you can use to specify the border color for negative data bars. |
|[GetBorderColorType](./getbordercolortype/) | Gets whether to use the same border color as positive data bars. |
|[SetBorderColorType](./setbordercolortype/) | Gets whether to use the same border color as positive data bars. |
|[GetColor](./getcolor/) | Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars. |
|[SetColor](./setcolor/) | Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars. |
|[GetColorType](./getcolortype/) | Gets or sets whether to use the same fill color as positive data bars. |
|[SetColorType](./setcolortype/) | Gets or sets whether to use the same fill color as positive data bars. |
