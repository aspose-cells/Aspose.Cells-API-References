##RenameStrategy Enum
'RenameStrategy enum. Encapsulates the object that represents renamestrategy in Go.'
## RenameStrategy Enum
Strategy option for duplicate names of columns.
```go
type RenameStrategy int32
```
## Fields
| Field | Description |
| --- | --- |
|[Exception](./exception/) | Throws exception. |
|[Digit](./digit/) | Named with digit. Duplicated names will become ...1, ...2, etc. |
|[Letter](./letter/) | Named with letter.. Duplicated names will become ...A, ...B, etc. |
