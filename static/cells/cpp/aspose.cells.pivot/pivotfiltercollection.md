##Aspose::Cells::Pivot::PivotFilterCollection class
'Aspose::Cells::Pivot::PivotFilterCollection class. Represents a collection of all the PivotFilter objects in C++.'
## PivotFilterCollection class
Represents a collection of all the [PivotFilter](../pivotfilter/) objects.
```cpp
class PivotFilterCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(int32_t fieldIndex, PivotFilterType type)](./add/) |  **(Deprecated)** Adds a [PivotFilter](../pivotfilter/)[Object](../../aspose.cells/object/) to the specific type. |
| [AddDateFilter(int32_t baseFieldIndex, PivotFilterType type, const Date\& dateTime1, const Date\& dateTime2)](./adddatefilter/) | Filters by date setting of row or column pivot field. |
| [AddLabelFilter(int32_t baseFieldIndex, PivotFilterType type, const U16String\& label1, const U16String\& label2)](./addlabelfilter/) | Filters by captions of row or column pivot field. |
| [AddLabelFilter(int32_t baseFieldIndex, PivotFilterType type, const char16_t* label1, const char16_t* label2)](./addlabelfilter/) | Filters by captions of row or column pivot field. |
| [AddTop10Filter(int32_t baseFieldIndex, int32_t valueFieldIndex, PivotFilterType type, bool isTop, int32_t itemCount)](./addtop10filter/) | Filters by values of data pivot field. |
| [AddValueFilter(int32_t baseFieldIndex, int32_t valueFieldIndex, PivotFilterType type, double value1, double value2)](./addvaluefilter/) | Filters by values of data pivot field. |
| [ClearFilter(int32_t fieldIndex)](./clearfilter/) | Clear [PivotFilter](../pivotfilter/) from the specific [PivotField](../pivotfield/). |
| [Get(int32_t index)](./get/) | Gets the pivotfilter object at the specific index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotFilterCollection\& src)](./operator_asm/) | operator= |
| [PivotFilterCollection(PivotFilterCollection_Impl* impl)](./pivotfiltercollection/) | Constructs from an implementation object. |
| [PivotFilterCollection(const PivotFilterCollection\& src)](./pivotfiltercollection/) | Copy constructor. |
| [~PivotFilterCollection()](./~pivotfiltercollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
