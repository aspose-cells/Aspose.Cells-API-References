##Aspose::Cells::Slicers::SlicerCollection class
'Aspose::Cells::Slicers::SlicerCollection class. Specifies the collection of all the Slicer objects on the specified worksheet in C++.'
## SlicerCollection class
Specifies the collection of all the [Slicer](../slicer/) objects on the specified worksheet.
```cpp
class SlicerCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const PivotTable\& pivot, const U16String\& destCellName, const U16String\& baseFieldName)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const char16_t* destCellName, const char16_t* baseFieldName)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, int32_t row, int32_t column, const U16String\& baseFieldName)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, int32_t row, int32_t column, const char16_t* baseFieldName)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, int32_t row, int32_t column, int32_t baseFieldIndex)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const U16String\& destCellName, int32_t baseFieldIndex)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const char16_t* destCellName, int32_t baseFieldIndex)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, int32_t row, int32_t column, const PivotField\& baseField)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const U16String\& destCellName, const PivotField\& baseField)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const char16_t* destCellName, const PivotField\& baseField)](./add/) | Add a new [Slicer](../slicer/) using PivotTable as data source. |
| [Add(const ListObject\& table, int32_t index, const U16String\& destCellName)](./add/) | Add a new [Slicer](../slicer/) using ListObjet as data source. |
| [Add(const ListObject\& table, int32_t index, const char16_t* destCellName)](./add/) | Add a new [Slicer](../slicer/) using ListObjet as data source. |
| [Add(const ListObject\& table, const ListColumn\& listColumn, const U16String\& destCellName)](./add/) | Add a new [Slicer](../slicer/) using ListObjet as data source. |
| [Add(const ListObject\& table, const ListColumn\& listColumn, const char16_t* destCellName)](./add/) | Add a new [Slicer](../slicer/) using ListObjet as data source. |
| [Add(const ListObject\& table, const ListColumn\& listColumn, int32_t row, int32_t column)](./add/) | Add a new [Slicer](../slicer/) using ListObjet as data source. |
| [Clear()](./clear/) | Clear all [Slicers](../). |
| [Get(int32_t index)](./get/) | Gets the [Slicer](../slicer/) by index. |
| [Get(const U16String\& name)](./get/) | Gets the [Slicer](../slicer/) by slicer's name. |
| [Get(const char16_t* name)](./get/) | Gets the [Slicer](../slicer/) by slicer's name. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SlicerCollection\& src)](./operator_asm/) | operator= |
| [Remove(const Slicer\& slicer)](./remove/) | Remove the specified [Slicer](../slicer/). |
| [RemoveAt(int32_t index)](./removeat/) | Deletes the [Slicer](../slicer/) at the specified index. |
| [SlicerCollection(SlicerCollection_Impl* impl)](./slicercollection/) | Constructs from an implementation object. |
| [SlicerCollection(const SlicerCollection\& src)](./slicercollection/) | Copy constructor. |
| [~SlicerCollection()](./~slicercollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);
Cells cells = sheet.GetCells();
cells.Get(0, 0).PutValue(u"fruit");
cells.Get(1, 0).PutValue(u"grape");
cells.Get(2, 0).PutValue(u"blueberry");
cells.Get(3, 0).PutValue(u"kiwi");
cells.Get(4, 0).PutValue(u"cherry");
cells.Get(5, 0).PutValue(u"grape");
cells.Get(6, 0).PutValue(u"blueberry");
cells.Get(7, 0).PutValue(u"kiwi");
cells.Get(8, 0).PutValue(u"cherry");
cells.Get(0, 1).PutValue(u"year");
cells.Get(1, 1).PutValue(2020);
cells.Get(2, 1).PutValue(2020);
cells.Get(3, 1).PutValue(2020);
cells.Get(4, 1).PutValue(2020);
cells.Get(5, 1).PutValue(2021);
cells.Get(6, 1).PutValue(2021);
cells.Get(7, 1).PutValue(2021);
cells.Get(8, 1).PutValue(2021);
cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);
cells.Get(5, 2).PutValue(90);
cells.Get(6, 2).PutValue(100);
cells.Get(7, 2).PutValue(110);
cells.Get(8, 2).PutValue(120);
PivotTableCollection pivots = sheet.GetPivotTables();
int pivotIndex = pivots.Add(u"=Sheet1!A1:C9", u"A12", u"TestPivotTable");
PivotTable pivot = pivots.Get(pivotIndex);
pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"year");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");
pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);
pivot.RefreshData();
pivot.CalculateData();
SlicerCollection slicers = sheet.GetSlicers();
int tableIndex = sheet.GetListObjects().Add(u"A1", u"C9", true);
ListObject table = sheet.GetListObjects().Get(tableIndex);
book.Save("out.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Slicers](../)
* Library [Aspose.Cells for C++](../../)
