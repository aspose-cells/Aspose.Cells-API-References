##PivotPageFields Class
'PivotPageFields class. Encapsulates the object that represents pivotpagefields in Go.'
## PivotPageFields class
Represents the pivot page field itemsif the pivot table data source is consolidation ranges.It only can contain up to 4 fields.
```go
type PivotPageFields struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPivotPageFields](./newpivotpagefields/) | Represents the pivot page field items. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[AddPageField](./addpagefield/) | Adds a page field. |
|[GetPageFieldCount](./getpagefieldcount/) | Gets the number of page fields. |
|[AddIdentify](./addidentify/) | Sets which item label in each page field to use to identify the data range.The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first. |
