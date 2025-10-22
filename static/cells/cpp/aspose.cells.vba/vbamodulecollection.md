##Aspose::Cells::Vba::VbaModuleCollection class
'Aspose::Cells::Vba::VbaModuleCollection class. Represents the list of VbaModule in C++.'
## VbaModuleCollection class
Represents the list of [VbaModule](../vbamodule/)
```cpp
class VbaModuleCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const Worksheet\& sheet)](./add/) | Adds module for a worksheet. |
| [Add(VbaModuleType type, const U16String\& name)](./add/) | Adds module. |
| [Add(VbaModuleType type, const char16_t* name)](./add/) | Adds module. |
| [AddDesignerStorage(const U16String\& name, const Vector \<uint8_t\>\& data)](./adddesignerstorage/) |  |
| [AddDesignerStorage(const char16_t* name, const Vector \<uint8_t\>\& data)](./adddesignerstorage/) |  |
| [AddUserForm(const U16String\& name, const U16String\& codes, const Vector \<uint8_t\>\& designerStorage)](./adduserform/) | Inser user form into VBA Project. |
| [AddUserForm(const char16_t* name, const char16_t* codes, const Vector \<uint8_t\>\& designerStorage)](./adduserform/) | Inser user form into VBA Project. |
| [Get(int32_t index)](./get/) | Gets [VbaModule](../vbamodule/) in the list by the index. |
| [Get(const U16String\& name)](./get/) | Gets [VbaModule](../vbamodule/) in the list by the name. |
| [Get(const char16_t* name)](./get/) | Gets [VbaModule](../vbamodule/) in the list by the name. |
| [GetCount()](./getcount/) |  |
| [GetDesignerStorage(const U16String\& name)](./getdesignerstorage/) | Represents the data of Designer. |
| [GetDesignerStorage(const char16_t* name)](./getdesignerstorage/) | Represents the data of Designer. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const VbaModuleCollection\& src)](./operator_asm/) | operator= |
| [Remove(const Worksheet\& sheet)](./remove/) | Removes module for a worksheet. |
| [Remove(const U16String\& name)](./remove/) | Remove the module by the name. |
| [Remove(const char16_t* name)](./remove/) | Remove the module by the name. |
| [VbaModuleCollection(VbaModuleCollection_Impl* impl)](./vbamodulecollection/) | Constructs from an implementation object. |
| [VbaModuleCollection(const VbaModuleCollection\& src)](./vbamodulecollection/) | Copy constructor. |
| [~VbaModuleCollection()](./~vbamodulecollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
// Init VBA project.
VbaProject vbaProject = workbook.GetVbaProject();
// Add a new module.
vbaProject.GetModules().Add(VbaModuleType::Class, u"test");
//Saving the Excel file
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Vba](../)
* Library [Aspose.Cells for C++](../../)
