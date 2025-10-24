##Aspose::Cells::Pivot::PivotTableCollection class
'Aspose::Cells::Pivot::PivotTableCollection class. Represents the collection of all the PivotTable objects on the specified worksheet in C++.'
## PivotTableCollection class
Represents the collection of all the [PivotTable](../pivottable/) objects on the specified worksheet.
```cpp
class PivotTableCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(const U16String\& sourceData, const U16String\& destCellName, const U16String\& tableName)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const char16_t* sourceData, const char16_t* destCellName, const char16_t* tableName)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const U16String\& sourceData, const U16String\& destCellName, const U16String\& tableName, bool useSameSource)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const char16_t* sourceData, const char16_t* destCellName, const char16_t* tableName, bool useSameSource)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const U16String\& sourceData, int32_t row, int32_t column, const U16String\& tableName)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const char16_t* sourceData, int32_t row, int32_t column, const char16_t* tableName)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const U16String\& sourceData, int32_t row, int32_t column, const U16String\& tableName, bool useSameSource)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const char16_t* sourceData, int32_t row, int32_t column, const char16_t* tableName, bool useSameSource)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const U16String\& sourceData, int32_t row, int32_t column, const U16String\& tableName, bool useSameSource, bool isXlsClassic)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const char16_t* sourceData, int32_t row, int32_t column, const char16_t* tableName, bool useSameSource, bool isXlsClassic)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const U16String\& sourceData, const U16String\& cell, const U16String\& tableName, bool useSameSource, bool isXlsClassic)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const char16_t* sourceData, const char16_t* cell, const char16_t* tableName, bool useSameSource, bool isXlsClassic)](./add/) | Adds a new [PivotTable](../pivottable/). |
| [Add(const PivotTable\& pivotTable, const U16String\& destCellName, const U16String\& tableName)](./add/) | Adds a new [PivotTable](../pivottable/) based on another [PivotTable](../pivottable/). |
| [Add(const PivotTable\& pivotTable, const char16_t* destCellName, const char16_t* tableName)](./add/) | Adds a new [PivotTable](../pivottable/) based on another [PivotTable](../pivottable/). |
| [Add(const PivotTable\& pivotTable, int32_t row, int32_t column, const U16String\& tableName)](./add/) | Adds a new [PivotTable](../pivottable/) based on another [PivotTable](../pivottable/). |
| [Add(const PivotTable\& pivotTable, int32_t row, int32_t column, const char16_t* tableName)](./add/) | Adds a new [PivotTable](../pivottable/) based on another [PivotTable](../pivottable/). |
| [Add(const Vector \<U16String\>\& sourceData, bool isAutoPage, const PivotPageFields\& pageFields, const U16String\& destCellName, const U16String\& tableName)](./add/) | Adds a new [PivotTable](../pivottable/)[Object](../../aspose.cells/object/) to the collection with multiple consolidation ranges as data source. |
| [Add(const Vector \<U16String\>\& sourceData, bool isAutoPage, const PivotPageFields\& pageFields, const char16_t* destCellName, const char16_t* tableName)](./add/) | Adds a new [PivotTable](../pivottable/)[Object](../../aspose.cells/object/) to the collection with multiple consolidation ranges as data source. |
| [Add(const Vector \<U16String\>\& sourceData, bool isAutoPage, const PivotPageFields\& pageFields, int32_t row, int32_t column, const U16String\& tableName)](./add/) | Adds a new [PivotTable](../pivottable/)[Object](../../aspose.cells/object/) to the collection with multiple consolidation ranges as data source. |
| [Add(const Vector \<U16String\>\& sourceData, bool isAutoPage, const PivotPageFields\& pageFields, int32_t row, int32_t column, const char16_t* tableName)](./add/) | Adds a new [PivotTable](../pivottable/)[Object](../../aspose.cells/object/) to the collection with multiple consolidation ranges as data source. |
| [Clear()](./clear/) | Clear all pivot tables. |
| [Dispose()](./dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Get(int32_t index)](./get/) | Gets the [PivotTable](../pivottable/) report by index. |
| [Get(const U16String\& name)](./get/) | Gets the [PivotTable](../pivottable/) report by pivottable's name. |
| [Get(const char16_t* name)](./get/) | Gets the [PivotTable](../pivottable/) report by pivottable's name. |
| [Get(int32_t row, int32_t column)](./get/) | Gets the [PivotTable](../pivottable/) report by pivottable's position. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotTableCollection\& src)](./operator_asm/) | operator= |
| [PivotTableCollection(PivotTableCollection_Impl* impl)](./pivottablecollection/) | Constructs from an implementation object. |
| [PivotTableCollection(const PivotTableCollection\& src)](./pivottablecollection/) | Copy constructor. |
| [Remove(const PivotTable\& pivotTable)](./remove/) | Deletes the specified [PivotTable](../pivottable/) and delete the [PivotTable](../pivottable/) data. |
| [Remove(const PivotTable\& pivotTable, bool keepData)](./remove/) | Deletes the specified [PivotTable](../pivottable/). |
| [RemoveAt(int32_t index)](./removeat/) | Deletes the [PivotTable](../pivottable/) at the specified index and delete the [PivotTable](../pivottable/) data. |
| [RemoveAt(int32_t index, bool keepData)](./removeat/) | Deletes the [PivotTable](../pivottable/) at the specified index. |
| [~PivotTableCollection()](./~pivottablecollection/) | Destructor. |
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
//Change PivotField's attributes
PivotField rowField = pivot.GetRowFields().Get(0);
rowField.SetDisplayName(u"custom display name");
//Add PivotFilter
int index = pivot.GetPivotFilters().Add(0, PivotFilterType::Count);
PivotFilter filter = pivot.GetPivotFilters().Get(index);
filter.GetAutoFilter().FilterTop10(0, false, false, 2);
//Add PivotFormatCondition
int formatIndex = pivot.GetPivotFormatConditions().Add();
PivotFormatCondition pfc = pivot.GetPivotFormatConditions().Get(formatIndex);
FormatConditionCollection fcc = pfc.GetFormatConditions();
fcc.AddArea(pivot.GetDataBodyRange());
int idx = fcc.AddCondition(FormatConditionType::CellValue);
FormatCondition fc = fcc.Get(idx);
fc.SetFormula1(u"100");
fc.SetOperator(OperatorType::GreaterOrEqual);
fc.GetStyle().SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });//Red
pivot.RefreshData();
pivot.CalculateData();
book.Save("out.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
