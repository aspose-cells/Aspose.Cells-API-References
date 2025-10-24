##IconFilter Class
'IconFilter class. Encapsulates the object that represents iconfilter in Go.'
## IconFilter class
Represents icon filter.
```go
type IconFilter struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewIconFilter](./newiconfilter/) | Constructs from an Object convertible to this. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[ToObject](./toobject/) | Gets the Object. |
|[GetIconSetType](./geticonsettype/) | Gets and sets which icon set is used in the filter criteria. |
|[SetIconSetType](./seticonsettype/) | Gets and sets which icon set is used in the filter criteria. |
|[GetIconId](./geticonid/) | Gets and sets Zero-based index of an icon in an icon set. |
|[SetIconId](./seticonid/) | Gets and sets Zero-based index of an icon in an icon set. |
