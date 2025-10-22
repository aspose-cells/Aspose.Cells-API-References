##ReserveMissingPivotItemType Enum
'ReserveMissingPivotItemType enum. Encapsulates the object that represents reservemissingpivotitemtype in Go.'
## ReserveMissingPivotItemType Enum
Represents how to keep the missing pivot items.
```go
type ReserveMissingPivotItemType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Default](./default/) | Removes old missint pivot items and reserves visible items which the current data source does not contain as missing items. |
|[All](./all/) | Reserves all missing items. |
|[None](./none/) | Removes all missing pivot items. |
