##Aspose::Cells::CellWatchCollection class
'Aspose::Cells::CellWatchCollection class. Represents the collection of cells on this worksheet being watched in the ''watch window'' in C++.'
## CellWatchCollection class
Represents the collection of cells on this worksheet being watched in the 'watch window'.
```cpp
class CellWatchCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(int32_t row, int32_t column)](./add/) | Adds [CellWatch](../cellwatch/) with row and column. |
| [Add(const U16String\& cellName)](./add/) | Adds [CellWatch](../cellwatch/) with the name the of cell. |
| [Add(const char16_t* cellName)](./add/) | Adds [CellWatch](../cellwatch/) with the name the of cell. |
| [CellWatchCollection()](./cellwatchcollection/) | Default constructor. |
| [CellWatchCollection(CellWatchCollection_Impl* impl)](./cellwatchcollection/) | Constructs from an implementation object. |
| [CellWatchCollection(const CellWatchCollection\& src)](./cellwatchcollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets and sets [CellWatch](../cellwatch/) by index. |
| [Get(const U16String\& cellName)](./get/) | Gets and sets [CellWatch](../cellwatch/) by the name of the cell. |
| [Get(const char16_t* cellName)](./get/) | Gets and sets [CellWatch](../cellwatch/) by the name of the cell. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const CellWatchCollection\& src)](./operator_asm/) | operator= |
| [~CellWatchCollection()](./~cellwatchcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
// Get the first Worksheet.
Worksheet sheet = workbook.GetWorksheets().Get(0);
// Add Cell Watch Item into the watch window
sheet.GetCellWatches().Add(u"B2");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
