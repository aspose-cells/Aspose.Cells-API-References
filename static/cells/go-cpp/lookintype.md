##LookInType Enum
'LookInType enum. Encapsulates the object that represents lookintype in Go.'
## LookInType Enum
Represents look in type.
```go
type LookInType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Formulas](./formulas/) | Finds the searched object from formula(<see cref="Cell.Formula"/>) if the cell is formula,otherwise finds from cell's original value(same with <see cref="OriginalValues"/>). |
|[Values](./values/) | Finds object from cell's original value(<see cref="Cell.Value"/>)and formatted value(<see cref="Cell.StringValue"/>). |
|[ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | Ignores cells that are formula. For those cells that are not formula,it is same with <see cref="Values"/>. |
|[Comments](./comments/) | Finds object from cell's comment only. Ignores those cells that have no comment. |
|[OnlyFormulas](./onlyformulas/) | Ignores cells that are not formula. For those cells that are formula,finds the searched object from formula(<see cref="Cell.Formula"/>). |
|[OriginalValues](./originalvalues/) | Find object from cell's original value only. |
|[FormattedValues](./formattedvalues/) | Find object from cell's formatted value(<see cref="Cell.StringValue"/>) only. |
