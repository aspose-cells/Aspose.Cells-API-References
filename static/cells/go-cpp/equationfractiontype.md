##EquationFractionType Enum
'EquationFractionType enum. Encapsulates the object that represents equationfractiontype in Go.'
## EquationFractionType Enum
This specifies the display style of the fraction bar.
```go
type EquationFractionType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Bar](./bar/) | This specifies that the numerator is above and the denominator below is separated by a bar in the middle. |
|[NoBar](./nobar/) | This specifies that the numerator is above and the denominator below is not separated by a bar in the middle. |
|[Linear](./linear/) | This specifies that the numerator is on the left and the denominator is on the right, separated by a '/' in between. |
|[Skewed](./skewed/) | This specifies that the numerator is on the upper left and the denominator is on the lower right, separated by a "/". |
