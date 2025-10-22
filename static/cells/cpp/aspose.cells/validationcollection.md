##Aspose::Cells::ValidationCollection class
'Aspose::Cells::ValidationCollection class. Represents data validation collection in C++.'
## ValidationCollection class
Represents data validation collection.
```cpp
class ValidationCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const CellArea\& ca)](./add/) | Adds a data validation to the collection. |
| [Get(int32_t index)](./get/) | Gets the [Validation](../validation/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [GetValidationInCell(int32_t row, int32_t column)](./getvalidationincell/) | Gets the validation applied to given cell. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ValidationCollection\& src)](./operator_asm/) | operator= |
| [RemoveACell(int32_t row, int32_t column)](./removeacell/) | Removes all validation setting on the cell. |
| [RemoveArea(const CellArea\& ca)](./removearea/) | Removes all validation setting on the range.. |
| [ValidationCollection(ValidationCollection_Impl* impl)](./validationcollection/) | Constructs from an implementation object. |
| [ValidationCollection(const ValidationCollection\& src)](./validationcollection/) | Copy constructor. |
| [~ValidationCollection()](./~validationcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
ValidationCollection validations = workbook.GetWorksheets().Get(0).GetValidations();
CellArea area = CellArea::CreateCellArea(0, 0, 1, 1);
Validation validation = validations.Get(validations.Add(area));
validation.SetType(ValidationType::List);
validation.SetFormula1(u"a,b,c,d");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
