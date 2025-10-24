##Aspose::Cells::Rendering::SheetSet class
'Aspose::Cells::Rendering::SheetSet class. Describes a set of sheets in C++.'
## SheetSet class
Describes a set of sheets.
```cpp
class SheetSet
```
## Methods
| Method | Description |
| --- | --- |
| static [GetActive()](./getactive/) | Gets a set with active sheet of the workbook. |
| static [GetAll()](./getall/) | Gets a set with all sheets of the workbook in their original order. |
| static [GetVisible()](./getvisible/) | Gets a set with visible sheets of the workbook in their original order. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SheetSet\& src)](./operator_asm/) | operator= |
| explicit [SheetSet(const Vector \<int32_t\>\& sheetIndexes)](./sheetset/) | Creates a sheet set based on exact sheet indexes. |
| explicit [SheetSet(const Vector \<U16String\>\& sheetNames)](./sheetset/) | Creates a sheet set based on exact sheet names. |
| [SheetSet(SheetSet_Impl* impl)](./sheetset/) | Constructs from an implementation object. |
| [SheetSet(const SheetSet\& src)](./sheetset/) | Copy constructor. |
| [~SheetSet()](./~sheetset/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Rendering](../)
* Library [Aspose.Cells for C++](../../)
