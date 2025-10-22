##Aspose::Cells::NameCollection class
'Aspose::Cells::NameCollection class. Represents a collection of all the Name objects in the spreadsheet in C++.'
## NameCollection class
Represents a collection of all the [Name](../name/) objects in the spreadsheet.
```cpp
class NameCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const U16String\& text)](./add/) | Defines a new name. |
| [Add(const char16_t* text)](./add/) | Defines a new name. |
| [Clear()](./clear/) | Remove all defined names which are not referenced by the formulas and data source. If the defined name is referred, we only set Name.ReferTo as null and hide them. |
| [Filter(NameScopeType type, int32_t sheetIndex)](./filter/) | Gets all defined name by scope. |
| [Get(int32_t index)](./get/) | Gets the [Name](../name/) element at the specified index. |
| [Get(const U16String\& text)](./get/) | Gets the [Name](../name/) element with the specified name. |
| [Get(const char16_t* text)](./get/) | Gets the [Name](../name/) element with the specified name. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [NameCollection(NameCollection_Impl* impl)](./namecollection/) | Constructs from an implementation object. |
| [NameCollection(const NameCollection\& src)](./namecollection/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const NameCollection\& src)](./operator_asm/) | operator= |
| [Remove(const Vector \<U16String\>\& names)](./remove/) | Remove an array of name. |
| [Remove(const U16String\& text)](./remove/) | Remove the name. |
| [Remove(const char16_t* text)](./remove/) | Remove the name. |
| [RemoveAt(int32_t index)](./removeat/) | Remove the name at the specific index. |
| [RemoveDuplicateNames()](./removeduplicatenames/) | Remove the duplicate defined names. |
| [Sort()](./sort/) | Sorts defined names. |
| [~NameCollection()](./~namecollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
