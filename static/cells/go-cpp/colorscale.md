##ColorScale Class
'ColorScale class. Encapsulates the object that represents colorscale in Go.'
## ColorScale class
Describe the ColorScale conditional formatting rule.This conditional formatting rule creates a gradated color scale on the cells.
```go
type ColorScale struct  {
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
|[GetIs3ColorScale](./getis3colorscale/) | Indicates whether conditional formatting is 3 color scale. |
|[SetIs3ColorScale](./setis3colorscale/) | Indicates whether conditional formatting is 3 color scale. |
|[GetMinCfvo](./getmincfvo/) | Get or set this ColorScale's min value object.Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
|[GetMidCfvo](./getmidcfvo/) | Get or set this ColorScale's mid value object.Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it. |
|[GetMaxCfvo](./getmaxcfvo/) | Get or set this ColorScale's max value object.Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
|[GetMinColor](./getmincolor/) | Get or set the gradient color for the minimum value in the range. |
|[SetMinColor](./setmincolor/) | Get or set the gradient color for the minimum value in the range. |
|[GetMidColor](./getmidcolor/) | Get or set the gradient color for the middle value in the range. |
|[SetMidColor](./setmidcolor/) | Get or set the gradient color for the middle value in the range. |
|[GetMaxColor](./getmaxcolor/) | Get or set the gradient color for the maximum value in the range. |
|[SetMaxColor](./setmaxcolor/) | Get or set the gradient color for the maximum value in the range. |
