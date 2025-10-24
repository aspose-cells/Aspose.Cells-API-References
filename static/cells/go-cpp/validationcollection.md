##ValidationCollection Class
'ValidationCollection class. Encapsulates the object that represents validationcollection in Go.'
## ValidationCollection class
Represents data validation collection.
```go
type ValidationCollection struct  {
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
|[Add](./add/) | Adds a data validation to the collection. |
|[Get](./get/) | Gets the Validation element at the specified index. |
|[RemoveACell](./removeacell/) | Removes all validation setting on the cell. |
|[RemoveArea](./removearea/) | Removes all validation setting on the range.. |
|[GetValidationInCell](./getvalidationincell/) | Gets the validation applied to given cell. |
|[GetCount](./getcount/) |  |
