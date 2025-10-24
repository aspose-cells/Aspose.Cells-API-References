##Aspose::Cells::Tables::ListObjectCollection class
'Aspose::Cells::Tables::ListObjectCollection class. Represents a collection of ListObject objects in the worksheet in C++.'
## ListObjectCollection class
Represents a collection of [ListObject](../listobject/) objects in the worksheet.
```cpp
class ListObjectCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn, bool hasHeaders)](./add/) | Adds a [ListObject](../listobject/) to the worksheet. |
| [Add(const U16String\& startCell, const U16String\& endCell, bool hasHeaders)](./add/) | Adds a [ListObject](../listobject/) to the worksheet. |
| [Add(const char16_t* startCell, const char16_t* endCell, bool hasHeaders)](./add/) | Adds a [ListObject](../listobject/) to the worksheet. |
| [Get(int32_t index)](./get/) | Gets the [ListObject](../listobject/) by index. |
| [Get(const U16String\& tableName)](./get/) | Gets the [ListObject](../listobject/) by specified name. |
| [Get(const char16_t* tableName)](./get/) | Gets the [ListObject](../listobject/) by specified name. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [ListObjectCollection(ListObjectCollection_Impl* impl)](./listobjectcollection/) | Constructs from an implementation object. |
| [ListObjectCollection(const ListObjectCollection\& src)](./listobjectcollection/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ListObjectCollection\& src)](./operator_asm/) | operator= |
| [UpdateColumnName()](./updatecolumnname/) | Update all column name of the tables. |
| [~ListObjectCollection()](./~listobjectcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Tables](../)
* Library [Aspose.Cells for C++](../../)
