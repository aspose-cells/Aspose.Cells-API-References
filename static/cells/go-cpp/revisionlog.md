##RevisionLog Class
'RevisionLog class. Encapsulates the object that represents revisionlog in Go.'
## RevisionLog class
Represents the revision log.
```go
type RevisionLog struct  {
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
|[GetMetadataTable](./getmetadatatable/) | Gets table that contains metadata about a list of specific changes that have taken placefor this workbook. |
|[GetRevisions](./getrevisions/) | Gets all revisions in this log. |
