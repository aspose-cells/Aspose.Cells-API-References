##UpdateLinksType Enum
'UpdateLinksType enum. Encapsulates the object that represents updatelinkstype in Go.'
## UpdateLinksType Enum
Represents how to update links to other workbooks when the workbook is opened.
```go
type UpdateLinksType int32
```
## Fields
| Field | Description |
| --- | --- |
|[UserSet](./userset/) | Prompt user to update. |
|[Never](./never/) | Do not update, and do not prompt user. |
|[Always](./always/) | Always update. |
