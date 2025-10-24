##PivotConditionFormatRuleType Enum
'PivotConditionFormatRuleType enum. Encapsulates the object that represents pivotconditionformatruletype in Go.'
## PivotConditionFormatRuleType Enum
Represents PivotTable condition formatting rule type.
```go
type PivotConditionFormatRuleType int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | Indicates that Top N conditional formatting is not evaluated |
|[All](./all/) | Indicates that Top N conditional formatting isevaluated across the entire scope range. |
|[Row](./row/) | Indicates that Top N conditional formatting is evaluated for each row. |
|[Column](./column/) | Indicates that Top N conditional formatting isevaluated for each column. |
