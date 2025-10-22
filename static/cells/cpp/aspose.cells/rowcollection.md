##Aspose::Cells::RowCollection class
'Aspose::Cells::RowCollection class. Collects the Row objects that represent the individual rows in a worksheet in C++.'
## RowCollection class
Collects the [Row](../row/) objects that represent the individual rows in a worksheet.
```cpp
class RowCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Clear()](./clear/) | Clear all rows and cells. |
| [Get(int32_t rowIndex)](./get/) | Gets a [Row](../row/) object by given row index. The [Row](../row/) object of given row index will be instantiated if it does not exist before. |
| [GetCount()](./getcount/) | Gets the number of rows in this collection. |
| [GetEnumerator()](./getenumerator/) | Gets an enumerator that iterates rows through this collection. |
| [GetEnumerator(bool reversed, bool sync)](./getenumerator/) | Gets an enumerator that iterates rows through this collection. |
| [GetRowByIndex(int32_t index)](./getrowbyindex/) | Gets the row object by the position in the list. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const RowCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Remove the row item at the specified index(position) in this collection. |
| [RowCollection(RowCollection_Impl* impl)](./rowcollection/) | Constructs from an implementation object. |
| [RowCollection(const RowCollection\& src)](./rowcollection/) | Copy constructor. |
| [~RowCollection()](./~rowcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Get first row
Row row = worksheet.GetCells().GetRows().Get(0);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
