##VbaModuleCollection Class
'VbaModuleCollection class. Encapsulates the object that represents vbamodulecollection in Go.'
## VbaModuleCollection class
Represents the list of <see cref="VbaModule"/>
```go
type VbaModuleCollection struct  {
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
|[AddDesignerStorage](./adddesignerstorage/) |  |
|[GetDesignerStorage](./getdesignerstorage/) | Represents the data of Designer. |
|[Add_Worksheet](./add_worksheet/) | Adds module for a worksheet. |
|[Add_VbaModuleType_String](./add_vbamoduletype_string/) | Adds module. |
|[AddUserForm](./adduserform/) | Inser user form into VBA Project. |
|[Get_Int](./get_int/) | Gets VbaModule in the list by the index. |
|[Remove_Worksheet](./remove_worksheet/) | Removes module for a worksheet. |
|[Remove_String](./remove_string/) | Remove the module by the name |
|[Get_String](./get_string/) | Gets VbaModule in the list by the name. |
|[GetCount](./getcount/) |  |
