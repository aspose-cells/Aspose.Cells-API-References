##SlicerCache Class
'SlicerCache class. Encapsulates the object that represents slicercache in Go.'
## SlicerCache class
Represent summary description of slicer cache
```go
type SlicerCache struct  {
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
|[GetCrossFilterType](./getcrossfiltertype/) | Returns or sets whether a slicer is participating in cross filtering with other slicersthat share the same slicer cache, and how cross filtering is displayed. Read/write |
|[SetCrossFilterType](./setcrossfiltertype/) | Returns or sets whether a slicer is participating in cross filtering with other slicersthat share the same slicer cache, and how cross filtering is displayed. Read/write |
|[GetList](./getlist/) | Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only |
|[GetSlicerCacheItems](./getslicercacheitems/) | Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only |
|[GetName](./getname/) | Returns the name of the slicer cache. |
|[GetSourceName](./getsourcename/) | Returns the name of this slicer cache. |
