##ResourceLoadingType Enum
'ResourceLoadingType enum. Encapsulates the object that represents resourceloadingtype in Go.'
## ResourceLoadingType Enum
Represents how to loading the linked resource.
```go
type ResourceLoadingType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Default](./default/) | Loads this resource as usual. |
|[Skip](./skip/) | Skips loading of this resource. |
|[UserProvided](./userprovided/) | Use stream provided by user |
