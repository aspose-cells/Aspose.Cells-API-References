##PivotMissingItemLimitType Enum
'PivotMissingItemLimitType enum. Encapsulates the object that represents pivotmissingitemlimittype in Go.'
## PivotMissingItemLimitType Enum
Represents number of items to retain per field.
```go
type PivotMissingItemLimitType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Automatic](./automatic/) | The default number of unique items per PivotField allowed. |
|[Max](./max/) | The maximum number of unique items per PivotField allowed (>32,500). |
|[None](./none/) | No unique items per PivotField allowed. |
