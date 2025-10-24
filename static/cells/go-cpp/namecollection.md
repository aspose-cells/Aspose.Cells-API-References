##NameCollection Class
'NameCollection class. Encapsulates the object that represents namecollection in Go.'
## NameCollection class
Represents a collection of all the <see cref="Name"/> objects in the spreadsheet.
```go
type NameCollection struct  {
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
|[Add](./add/) | Defines a new name. |
|[Get_Int](./get_int/) | Gets the Name element at the specified index. |
|[Filter](./filter/) | Gets all defined name by scope. |
|[Get_String](./get_string/) | Gets the Name element with the specified name. |
|[Remove_stringArray](./remove_stringarray/) | Remove an array of name |
|[Remove_String](./remove_string/) | Remove the name. |
|[RemoveAt](./removeat/) | Remove the name at the specific index. |
|[Clear](./clear/) | Remove all defined names which are not referenced by the formulas and data source.If the defined name is referred, we only set Name.ReferTo as null and hide them. |
|[RemoveDuplicateNames](./removeduplicatenames/) | Remove the duplicate defined names |
|[Sort](./sort/) | Sorts defined names. |
|[GetCount](./getcount/) |  |
