##SlicerCacheCrossFilterType Enum
'SlicerCacheCrossFilterType enum. Encapsulates the object that represents slicercachecrossfiltertype in Go.'
## SlicerCacheCrossFilterType Enum
Represent the type of SlicerCacheCrossFilterType
```go
type SlicerCacheCrossFilterType int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | The table style element of the slicer style for slicer itemswith no data is not applied to slicer items with no data, and slicer itemswith no data are not sorted separately in the list of slicer items in the slicer view |
|[ShowItemsWithDataAtTop](./showitemswithdataattop/) | The table style element of the slicer style for slicer items withno data is applied to slicer items with no data, and slicer itemswith no data are sorted at the bottom in the list of slicer items in the slicer view |
|[ShowItemsWithNoData](./showitemswithnodata/) | The table style element of the slicer style for slicer items with no datais applied to slicer items with no data, and slicer items with no dataare not sorted separately in the list of slicer items in the slicer view. |
