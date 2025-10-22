##DataSorterKey Class
'DataSorterKey class. Encapsulates the object that represents datasorterkey in Go.'
## DataSorterKey class
Represents the key of the data sorter.
```go
type DataSorterKey struct  {
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
|[GetOrder](./getorder/) | Indicates the order of sorting. |
|[GetIndex](./getindex/) | Gets the sorted column index(absolute position, column A is 0, B is 1, ...). |
|[GetType](./gettype/) | Represents the type of sorting. |
|[GetIconSetType](./geticonsettype/) | Represents the icon set type. |
|[GetIconId](./geticonid/) | Represents the id of the icon set type. |
|[GetColor](./getcolor/) | Gets the sorted color. |
