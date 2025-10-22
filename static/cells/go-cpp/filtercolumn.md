##FilterColumn Class
'FilterColumn class. Encapsulates the object that represents filtercolumn in Go.'
## FilterColumn class
Represents a filter for a single column. The Filter object is a member of the Filters collection
```go
type FilterColumn struct  {
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
|[IsDropdownVisible](./isdropdownvisible/) | Indicates whether the AutoFilter button for this column is visible. |
|[SetIsDropdownVisible](./setisdropdownvisible/) | Indicates whether the AutoFilter button for this column is visible. |
|[GetFilter](./getfilter/) | Gets and sets the condition of filtering data. |
|[SetFilter](./setfilter/) | Gets and sets the condition of filtering data. |
|[GetFilterType](./getfiltertype/) | Gets and sets the type fo filtering data. |
|[SetFilterType](./setfiltertype/) | Gets and sets the type fo filtering data. |
|[GetFieldIndex](./getfieldindex/) | Gets and sets the column offset in the range. |
|[SetFieldIndex](./setfieldindex/) | Gets and sets the column offset in the range. |
