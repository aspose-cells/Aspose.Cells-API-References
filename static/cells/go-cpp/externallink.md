##ExternalLink Class
'ExternalLink class. Encapsulates the object that represents externallink in Go.'
## ExternalLink class
Represents an external link in a workbook.
```go
type ExternalLink struct  {
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
|[GetType](./gettype/) | Gets the type of external link. |
|[GetPathType](./getpathtype/) | Get the path type of this external link |
|[GetOriginalDataSource](./getoriginaldatasource/) | Represents stored data source of the external link. |
|[SetOriginalDataSource](./setoriginaldatasource/) | Represents stored data source of the external link. |
|[GetDataSource](./getdatasource/) | Represents data source of the external link. |
|[SetDataSource](./setdatasource/) | Represents data source of the external link. |
|[AddExternalName](./addexternalname/) | Adds an external name. |
|[IsReferred](./isreferred/) | Indicates whether this external link is referenced by others. |
|[IsVisible](./isvisible/) | Indicates whether this external link is visible in MS Excel. |
