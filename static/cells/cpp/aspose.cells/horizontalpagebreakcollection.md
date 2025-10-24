##Aspose::Cells::HorizontalPageBreakCollection class
'Aspose::Cells::HorizontalPageBreakCollection class. Encapsulates a collection of HorizontalPageBreak objects in C++.'
## HorizontalPageBreakCollection class
Encapsulates a collection of [HorizontalPageBreak](../horizontalpagebreak/) objects.
```cpp
class HorizontalPageBreakCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(int32_t row, int32_t startColumn, int32_t endColumn)](./add/) | Adds a horizontal page break to the collection. |
| [Add(int32_t row)](./add/) | Adds a horizontal page break to the collection. |
| [Add(int32_t row, int32_t column)](./add/) | Adds a horizontal page break to the collection. |
| [Add(const U16String\& cellName)](./add/) | Adds a horizontal page break to the collection. |
| [Add(const char16_t* cellName)](./add/) | Adds a horizontal page break to the collection. |
| [Get(int32_t index)](./get/) | Gets the [HorizontalPageBreak](../horizontalpagebreak/) element at the specified index. |
| [Get(const U16String\& cellName)](./get/) | Gets the [HorizontalPageBreak](../horizontalpagebreak/) element with the specified cell name. |
| [Get(const char16_t* cellName)](./get/) | Gets the [HorizontalPageBreak](../horizontalpagebreak/) element with the specified cell name. |
| [GetCount()](./getcount/) |  |
| [HorizontalPageBreakCollection(HorizontalPageBreakCollection_Impl* impl)](./horizontalpagebreakcollection/) | Constructs from an implementation object. |
| [HorizontalPageBreakCollection(const HorizontalPageBreakCollection\& src)](./horizontalpagebreakcollection/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const HorizontalPageBreakCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Removes the HPageBreak element at a specified name. |
| [~HorizontalPageBreakCollection()](./~horizontalpagebreakcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
//Add a pagebreak at G5
excel.GetWorksheets().Get(0).GetHorizontalPageBreaks().Add(u"G5");
excel.GetWorksheets().Get(0).GetVerticalPageBreaks().Add(u"G5");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
