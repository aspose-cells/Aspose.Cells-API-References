##FormatConditionValueType Enum
'FormatConditionValueType enum. Encapsulates the object that represents formatconditionvaluetype in Go.'
## FormatConditionValueType Enum
Condition value type.
```go
type FormatConditionValueType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Formula](./formula/) | The minimum/ midpoint / maximum value for thegradient is determined by a formula. |
|[Max](./max/) | Indicates that the maximum value in the range shall beused as the maximum value for the gradient. |
|[Min](./min/) | Indicates that the minimum value in the range shall beused as the minimum value for the gradient. |
|[Number](./number/) | Indicates that the minimum / midpoint / maximumvalue for the gradient is specified by a constantnumeric value. |
|[Percent](./percent/) | Value indicates a percentage between the minimumand maximum values in the range shall be used as theminimum / midpoint / maximum value for the gradient. |
|[Percentile](./percentile/) | Value indicates a percentile ranking in the range shallbe used as the minimum / midpoint / maximum valuefor the gradient. |
|[AutomaticMax](./automaticmax/) | Indicates that the Automatic maximum value in the range shall beused as the Automatic maximum value for the gradient. |
|[AutomaticMin](./automaticmin/) | Indicates that the Automatic minimum value in the range shall beused as the Automatic minimum value for the gradient. |
