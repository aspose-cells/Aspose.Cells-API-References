##ConditionalFormattingValue Class
'ConditionalFormattingValue class. Encapsulates the object that represents conditionalformattingvalue in Go.'
## ConditionalFormattingValue class
Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.
```go
type ConditionalFormattingValue struct  {
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
|[GetValue](./getvalue/) | Get or set the value of this conditional formatting value object.It should be used in conjunction with Type. |
|[SetValue](./setvalue/) | Get or set the value of this conditional formatting value object.It should be used in conjunction with Type. |
|[GetType](./gettype/) | Get or set the type of this conditional formatting value object.Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Maxwill auto set "Value" to null. |
|[SetType](./settype/) | Get or set the type of this conditional formatting value object.Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Maxwill auto set "Value" to null. |
|[IsGTE](./isgte/) | Get or set the Greater Than Or Equal flag.Use only for icon sets, determines whether this threshold value usesthe greater than or equal to operator.'false' indicates 'greater than' is used instead of 'greater than or equal to'.Default value is true. |
|[SetIsGTE](./setisgte/) | Get or set the Greater Than Or Equal flag.Use only for icon sets, determines whether this threshold value usesthe greater than or equal to operator.'false' indicates 'greater than' is used instead of 'greater than or equal to'.Default value is true. |
