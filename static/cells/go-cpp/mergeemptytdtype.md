##MergeEmptyTdType Enum
'MergeEmptyTdType enum. Encapsulates the object that represents mergeemptytdtype in Go.'
## MergeEmptyTdType Enum
Represents the merge type for empty TD element when exporting file to html.
```go
type MergeEmptyTdType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Default](./default/) | Display like MS Excel. |
|[None](./none/) | Empty TD elements will not be merged when exporting file to html.This will generate a significantly larger html file. |
|[MergeForcely](./mergeforcely/) | Merging empty TD element forcedly when exporting file to html.The size of html file will be reduced significantly after setting value to true.If you want to import the html file to excel or export perfect grid lines when saving file to html,please keep the default value. |
